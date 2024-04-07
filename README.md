# serverSetup
to setup a linux server for hunter
------------------

## go install

1. GOVERSION="1.22.1"
2. sudo rm -rf /usr/local/go ; sudo rm -rf $HOME/go; sudo rm -rf /bin/go
3. wget "[https://golang.org/dl/go${GOVERSION}.linux-amd64.tar.gz](https://golang.org/dl/go$%7BGOVERSION%7D.linux-amd64.tar.gz)" -4
4. tar -C /usr/local -xvf "go${GOVERSION}.linux-amd64.tar.gz"
5. echo "export PATH=$PATH:/usr/local/go/bin" >> ~/.zshrc
6. echo "export PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin:/bin:/root/go/bin:/usr/local/go/bin" >> ~/.zshrc
7. echo "export GOPATH=$HOME/go" >> ~/.zshrc
8. echo "export PATH=/usr/local/go/bin:$PATH:$GOPATH/bin" >> ~/.zshrc
9. source ~/.zshrc
10. go version

## required package

1. apt install vim curl zsh git net-tools tmux build-essential make python3-apt python3-distutils libssl-dev curl zsh git vim jq
2. Curl https://bootstrap.pypa.io/get-pip.py -o [get-pip.py](http://get-pip.py/); python3 [get-pip.py](http://get-pip.py/) ; rm [get-pip.py](http://get-pip.py/)

## Tools:

go install -v [github.com/projectdiscovery/subfinder/v2/cmd/subfinder@latest](http://github.com/projectdiscovery/subfinder/v2/cmd/subfinder@latest)
go install -v [github.com/projectdiscovery/mapcidr/cmd/mapcidr@latest](http://github.com/projectdiscovery/mapcidr/cmd/mapcidr@latest)
go install -v [github.com/projectdiscovery/httpx/cmd/httpx@latest](http://github.com/projectdiscovery/httpx/cmd/httpx@latest)
go install -v [github.com/projectdiscovery/katana/cmd/katana@latest](http://github.com/projectdiscovery/katana/cmd/katana@latest)
go install -v [github.com/projectdiscovery/notify/cmd/notify@latest](http://github.com/projectdiscovery/notify/cmd/notify@latest)
go install -v [github.com/projectdiscovery/dnsx/cmd/dnsx@latest](http://github.com/projectdiscovery/dnsx/cmd/dnsx@latest)
go install -v [github.com/projectdiscovery/shuffledns/cmd/shuffledns@latest](http://github.com/projectdiscovery/shuffledns/cmd/shuffledns@latest)
go install -v [github.com/projectdiscovery/nuclei/v2/cmd/nuclei@latest](http://github.com/projectdiscovery/nuclei/v2/cmd/nuclei@latest)
go install -v [github.com/projectdiscovery/naabu/v2/cmd/naabu@latest](http://github.com/projectdiscovery/naabu/v2/cmd/naabu@latest)
go install -v [github.com/projectdiscovery/alterx/cmd/alterx@latest](http://github.com/projectdiscovery/alterx/cmd/alterx@latest)
go install -v [github.com/tomnomnom/unfurl@latest](http://github.com/tomnomnom/unfurl@latest)
go install -v [github.com/tomnomnom/anew@latest](http://github.com/tomnomnom/anew@latest)
go install -v [github.com/tomnomnom/waybackurls@latest](http://github.com/tomnomnom/waybackurls@latest)
go install -v [github.com/ffuf/ffuf/v2@latest](http://github.com/ffuf/ffuf/v2@latest)
go install -v [github.com/owasp-amass/amass/v4/](http://github.com/owasp-amass/amass/v4/)...@master
pip3 install uro

more Tools repos:

https://github.com/trufflesecurity/trufflehog

https://github.com/xnl-h4ck3r/waymore

https://github.com/EnableSecurity/wafw00f

https://github.com/laramies/theHarvester

- http parameter discovery
    
    https://github.com/s0md3v/Arjun
    
- OSINT tool that finds domains, subdomains, directories, endpoints and files for a given seed URL
    
    https://github.com/caio-ishikawa/netscout
    
- pentesters swiss knife
    
    [secator: The pentester's swiss knife](https://securityonline.info/secator-the-pentesters-swiss-knife/)
