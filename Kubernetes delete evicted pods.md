[[Kubernetes]]
`kubectl get pod | grep Evicted | awk '{print $1}' | xargs kubectl delete pod -n studytonight

`kubectl get pod | grep Evicted | awk '{print $1}'

`kubectl get pod -n a4t-3atool | grep Evicted | awk '{print $1}'     
`kubectl get pod -n a4t-amsys | grep Evicted | awk '{print $1}'
`kubectl get pod -n a4t-ascot | grep Evicted | awk '{print $1}'
`kubectl get pod -n a4t-ckdinfo | grep Evicted | awk '{print $1}'
`kubectl get pod -n a4t-drtool | grep Evicted | awk '{print $1}'
`kubectl get pod -n a4t-feed | grep Evicted | awk '{print $1}'
`kubectl get pod -n a4t-gato | grep Evicted | awk '{print $1}'
`kubectl get pod -n a4t-ntmc | grep Evicted | awk '{print $1}'
`kubectl get pod -n a4t-platin | grep Evicted | awk '{print $1}'
`kubectl get pod -n a4t-platinmi | grep Evicted | awk '{print $1}'
`kubectl get pod -n a4t-qsys | grep Evicted | awk '{print $1}'
`kubectl get pod -n a4t-sca | grep Evicted | awk '{print $1}'
`kubectl get pod -n a4t-spedfinder | grep Evicted | awk '{print $1}'
`kubectl get pod -n a4t-spedmail | grep Evicted | awk '{print $1}'
`kubectl get pod -n a4t-stampmgr | grep Evicted | awk '{print $1}'
`kubectl get pod -n a4t-tis | grep Evicted | awk '{print $1}'
`kubectl get pod -n a4t-v42 | grep Evicted | awk '{print $1}'
`kubectl get pod -n a4t-v42 | grep Evicted | awk '{print $1}'
`kubectl get pod -n a4t-wspdoku | grep Evicted | awk '{print $1}'

`kubectl get pod -n a4t-3atool | grep Evicted | awk '{print $1}' | xargs kubectl delete pod -n a4t-3atool  
`kubectl get pod -n a4t-amsys | grep Evicted | awk '{print $1}' | xargs kubectl delete pod -n a4t-amsys 
`kubectl get pod -n a4t-ascot | grep Evicted | awk '{print $1}' | xargs kubectl delete pod -n a4t-ascot 
`kubectl get pod -n a4t-ckdinfo | grep Evicted | awk '{print $1}' | xargs kubectl delete pod -n a4t-ckdinfo
`kubectl get pod -n a4t-drtool | grep Evicted | awk '{print $1}' | xargs kubectl delete pod -n a4t-drtool
`kubectl get pod -n a4t-feed | grep Evicted | awk '{print $1}' | xargs kubectl delete pod -n a4t-feed
`kubectl get pod -n a4t-gato | grep Evicted | awk '{print $1}' | xargs kubectl delete pod -n a4t-gato
`kubectl get pod -n a4t-ntmc | grep Evicted | awk '{print $1}' | xargs kubectl delete pod -n a4t-ntmc
`kubectl get pod -n a4t-platin | grep Evicted | awk '{print $1}' | xargs kubectl delete pod -n a4t-platin
`kubectl get pod -n a4t-platinmi | grep Evicted | awk '{print $1}' | xargs kubectl delete pod -n a4t-platinmi
`kubectl get pod -n a4t-qsys | grep Evicted | awk '{print $1}' | xargs kubectl delete pod -n a4t-qsys
`kubectl get pod -n a4t-sca | grep Evicted | awk '{print $1}' | xargs kubectl delete pod -n a4t-sca
`kubectl get pod -n a4t-spedfinder | grep Evicted | awk '{print $1}' | xargs kubectl delete pod -n a4t-spedfinder
`kubectl get pod -n a4t-spedmail | grep Evicted | awk '{print $1}' | xargs kubectl delete pod -n a4t-spedmail
`kubectl get pod -n a4t-stampmgr | grep Evicted | awk '{print $1}' | xargs kubectl delete pod -n a4t-stampmgr
`kubectl get pod -n a4t-tis | grep Evicted | awk '{print $1}' | xargs kubectl delete pod -n a4t-tis
`kubectl get pod -n a4t-v42 | grep Evicted | awk '{print $1}' | xargs kubectl delete pod -n a4t-v42
`kubectl get pod -n a4t-wspdoku | grep Evicted | awk '{print $1}' | xargs kubectl delete pod -n a4t-wspdoku

