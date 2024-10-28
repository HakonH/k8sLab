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

