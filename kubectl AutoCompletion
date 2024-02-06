# kubectl with ZSH (oh-my-zsh)

## How to configure

Use the following commands to add the kubectl autocomplete to zsh:

```shell
mkdir -p ~/.oh-my-zsh/custom/plugins/kubectl-autocomplete/
kubectl completion zsh > ~/.oh-my-zsh/custom/plugins/kubectl-autocomplete/kubectl-autocomplete.plugin.zsh
```

After that, edit your `~/.zshrc` to include the plugin `kubectl-autocomplete`, like so:

```
# ~/.zshrc
# ...
plugins=(kubectl-autocomplete)
```

## Optional: kubens and kubectx
[Kubectx](https://github.com/ahmetb/kubectx) is a great plugin for easily switching namespaces and contexts.

You can install it with these commands:
```shell
curl -LO https://raw.githubusercontent.com/ahmetb/kubectx/master/kubectx
curl -LO https://raw.githubusercontent.com/ahmetb/kubectx/master/kubens

sudo chmod +x ./{kubectx,kubens}
sudo mv ./{kubectx,kubens} /usr/local/bin/

mkdir -p ~/.oh-my-zsh/completions
curl -L https://raw.githubusercontent.com/ahmetb/kubectx/master/completion/kubectx.zsh -o ~/.oh-my-zsh/completions/_kubectx.zsh
curl -L https://raw.githubusercontent.com/ahmetb/kubectx/master/completion/kubens.zsh -o ~/.oh-my-zsh/completions/_kubens.zsh
```

## How to use it

Press tab after running the commands and you should get suggestions for the output
```shell
kubectl g<TAB>
kubectl get p<TAB>

kubens <TAB>
kubectx <TAB>
```