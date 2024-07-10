# cka-exam
1. Update the nginx image of the deployment NGINX to 1.19.8
   : kubectl set image deployment nginx nginx=nginx:1.19.8
2. Change the static pod path to /etc/kubernetes/manifest
   : ps -aux | grep kubelet
    now copy the config yaml file here, /var/lib/kubelet/config.yaml
   : nano /var/lib/kubelet/config.yaml
   update the path staticPodPath: /etc/kubernetes/manifests
3. Upgrade the cluster:
   - kubeadm: 1.19.0
   - kubelet: 1.19.0
   - kubectl: 1.19.0  
   
