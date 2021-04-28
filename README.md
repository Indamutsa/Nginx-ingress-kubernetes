In this project is about setting up kubernetes ingress using nginx
It is a demo for a quick refresh to get started


#### You will need to enable ingress on minikube
-------------

Run: kubectl apply -f ./
Well make sure, you run one ingress. In case, there is a problem with webhook, delete it
>> kubectl delete -A ValidatingWebhookConfiguration ingress-nginx-admission

You will need to enable the host name locally <br>
On linux   run:

>> sudo vim /etc/hosts

before you need to run:

>> kube get ing


It might take a while to get the ip, so you may watch, once you have the ip
copy in that in hosts file as it is with localhsot set on 127.0.1.1

That's all. You can set both the path and the domains
