# GKE_Dimensionar_PVC´s
Aumentar o armazenamento de 30 PVC´s em um StatefulSet no Kubernetes. SEM DOWNTIME!!

## SEGUE O PASSO A PASSO:
1º Reduza as réplicas para 1 (mantendo apenas web-0)  :    kubectl scale statefulset web --replicas=1 

2º Use os seguintes parametros em seu arquivo statefulset2.yaml (arquivo esta no repositório)  

3º Execute o arquivo .yaml com o parametro --force (kubectl apply -f statefulset.yaml --force)


## DICA: Domine esses 3 conceitos para StatefulSets: 

PersistentVolumeClaimRetentionPolicy

UpdateStrategy com partition

Rolling Updates ordenados
