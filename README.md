# Start
This project has been taken from free Hydra jekyll theme
# Modified notes
- `bundle exec jekyll serve --host 0.0.0.0 --livereload`

# Gotchas
If running on Ruby 3.0 and get the error like `LoadError: cannot load such file -- webrick` , then do the following   (This is ONLY for local - github doesn't require this)

- `bundle add webrick`

# Serving in github pages
- Add your code to either organization or personal github (zet-go.github.io to techsparks.github.io)
- Go to zet-go.github.io > Settings > Pages and go with defaults
- In the custom domain add "www.zet-go.com" 
- Add CNAME record www -> techsparks.github.io 
- Sometimes we might need to add A records to point to 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153 e.g. A, @ , 185.199.108.153 in godaddy DNS
- After this github pages will add a CNAME file to the repo
- Finally SSL/TLS certificate is provisioned - this might take a while
- Have patience for about 10-15 and access https://zet-go.com or https://www.zet-go.com
