# ppaDemo

todo: set up gpg key for signing
see https://stackoverflow.com/questions/61096521/how-to-use-gpg-key-in-github-actions


```
curl -s --compressed "https://jaypi4c.github.io/ppaDemo/ubuntu/KEY.gpg" | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/jaypi4cDemo.gpg >/dev/null
sudo curl -s --compressed -o /etc/apt/sources.list.d/jaypi4cDemo.list "https://jaypi4c.github.io/ppaDemo/ubuntu/jaypi4cDemo.list"
sudo apt update
```