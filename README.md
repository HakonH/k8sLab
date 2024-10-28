
git init

git remote add origin git@github.com:HakonH/k8sLab.git

git status

git pull origin fluxcd-2022

git status

## git config --global init.defaultBranch fluxcd-2022

git status

git branch -M fluxcd-2022

git status

code .


flux bootstrap github \
  --token-auth \
  --owner=HakonH \
  --repository=k8sLab \
  --path=kubernetes/fluxcd/repositories/infra-repo/clusters/dev-cluster \
  --personal \
  --branch fluxcd-2022
  
  flux bootstrap github \
  --token-auth \
  --owner=HakonH \
  --repository=k8sLab \
  --path=kubernetes/fluxcd/repositories/infra-repo/clusters/dev-cluster \
  --components-extra=image-reflector-controller,image-automation-controller \
  --personal \
  --branch fluxcd-2022

