# ltmk

for date use:
date +"%Y-%m-%dT%T+10:00"

to build:
brew install hugo
hugo version

cd ~/src
hugo new site ltmk
cd ltmk
git init

git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke.git themes/ananke
echo "theme = 'ananke'" >> hugo.toml
or
git submodule add -b main https://github.com/nunocoracao/blowfish.git themes/blowfish
echo "theme = 'blowfish'" >> hugo.toml

hugo new content content/posts/helloworld.md
echo "baseURL = 'https://foobar.org/'" >> hugo.toml
echo "languageCode = 'en-us'" >> hugo.toml
echo "title = 'Hello World'" >> hugo.toml
echo "theme = 'ananke'" >> hugo.toml
hugo server --buildDrafts (or -D)

git add *
git commit 
git remote add origin https://github.com/username/new_repo
git push -u origin main

hugo   # writes out to public/

/domains/telstramedia.net/public_html --> ~/src/html

https://my.silicomnetwork.com/index.php?fuse=home&view=dashboard

a.telstramedia.net
85.239.245.210
ns1 = ct1new.neodns.info
ns2 = ct2new.neodns.info

Control Panel
https://us10.neodns.info:2222
 
Hostname ftp
us10.neodns.info

