# DevOps-Minikube-Install-game-SupermarioBros

Disini saya akan sharing tentang tatacara cara install game super mario bros di locahost dengan minikube dengan Image yang tersedia di dockerhub

## Step 1
- running minikube
```bash
  minikube start
```
- respon di cli minikube sudah running
![Screenshot](https://drive.google.com/uc?id=1JrGSqj4ExV_CfWigA-UcQrmfSs6lWSn4)

## Step 2
- buka dashboard minikube
```bash
  minikube dashboard
```
- respon di cli berhasil running dashboard
![Screenshot](https://drive.google.com/uc?id=1JSohRpbp6rH-OXftIBV8VU82CJuLdVUb)
- dashboard sudah running
![Screenshot dahsbord](https://drive.google.com/uc?id=14IVd1dv8TFi5ZQUImSLWAoVl8Hpf5HXp)

## Step 3
- buka dockerhub, lalu cari game supermario
![Screenshot dahsbord](https://drive.google.com/uc?id=13SVivSkGa9O_rJu9Jb6yxaR6va0ONnqH)

## Step 4
- buka dashboard minikubenya lalu pilih deployment, lalu klik simbol (+) dan isikan coding untuk YAML dibawah ini
- codingnya
![Screenshot dahsbord](https://drive.google.com/uc?id=1S-3Sr6BGWrlpb-DG0G_3BSgU9djh-cqP)
- lalu klik upload dan tunggu diproses oleh minikubenya sampai supermario siap di gunakan dilokal
![Screenshot dahsbord](https://drive.google.com/uc?id=1qrzHFvfbKXzu9ddDm8qaEVsnvXUUCJfg)
- gambar diatas sedang deployment dan gambar dibawah deployment sudah selesai
![Screenshot dahsbord](https://drive.google.com/uc?id=1ndIg_pmy7k-v-Guxz3ot-dIin4FiB_2t)

## Step 5
- buka cli baru, trus ketik command dibawah ini untuk nama Podnya dan running podnya
```bash
  kubectl get pod
```
![Screenshot dahsbord](https://drive.google.com/uc?id=1jgblF45ZIVoiCu4M2v4qgFB_EPz8e_m9)
- lalu kita meneruskan port lokal ke port di Pod. 3000 port lokal, 8080 port containernya

```bash
  kubectl port-forward supermariobros-774bcbdf89-f4bgj 3000:8080
```
- nanti hasilnya seperti ini
<br />

![Screenshot dahsbord](https://drive.google.com/uc?id=1VXbHxWFBAlXn5Zc-noJhmtBiKJLd14RB)



## 🚀 About Me
Thankyou for read .. 
