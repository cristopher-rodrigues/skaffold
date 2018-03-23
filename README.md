# START

# DEPENDENCIES

```bash
curl -LO https://storage.googleapis.com/kubernetes-release/release/`curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt`/bin/darwin/amd64/kubectl
```
```bash
brew cask install minikube
```
```bash
brew cask install virtualbox
```
```bash
curl -Lo skaffold https://storage.googleapis.com/skaffold/releases/v0.2.0/skaffold-darwin-amd64 && chmod +x skaffold && sudo mv skaffold /usr/local/bin
```

## RUN

```bash
docker build .
```
```bash
minikube start
```
```bash
skaffold dev
```

In another terminal window

```bash
minikube service node-app
```
You can edit a index.js to show skaffold in action (to rebuild and reload kubernets environment)


