## User Creation Commands ##

```
mkdir -p  ~/.kube/users && cd ~/.kube/users
```

```
openssl genrsa -out client1.key 2048
```

```
openssl req -new -key client1.key -out client1.csr -subj "/CN=client1/O=tenant1"
```

```
openssl x509 -req -CA /home/deepu/atlan/tenant-user/ca.crt -CAkey /home/deepu/atlan/tenant-user/ca.key -CAcreateserial -days 730 -in client1.csr -out client1.crt
```

```
kubectl config set-credentials client1 --client-certificate=client1.crt --client-key=client1.key
```

```
kubectl config get-contexts
```

```
kubectl config use-context client1-kubernetes
```


