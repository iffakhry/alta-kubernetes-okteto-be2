# Kubernetes

- install kubectl
- register di okteto
- login ke okteto, masuk ke menu Setting -> setup -> kubernetes credentials (download file config)
- Load file config (via terminal)
    `export KUBECONFIG=$HOME/Downloads/okteto-kube.config:${KUBECONFIG:-$HOME/.kube/config}`

- Download guestbook-go example project `https://github.com/kubernetes/examples`
- buat folder manifest
- copy file *.json ke manifest
- run 
    `kubectl apply -f manifest` untuk deploy guestbook app
    `kubectl apply -f mytoko` untuk deploy mytoko app

- list command :
    ```
    - kubectl get pods
    - kubectl get services
    - kubectl get ingress
    ```

- delete 
    guestbook `kubectl delete replicationcontroller guestbook`
    mytoko `kubectl delete deployment mytoko`


