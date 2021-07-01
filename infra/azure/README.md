### Kubernetes dashboard command

```
kubectl create -f https://raw.githubusercontent.com/kubernetes/dashboard/v2.0.0/aio/deploy/recommended.yaml

kubectl proxy

http://localhost:8001/api/v1/namespaces/kubernetes-dashboard/services/https:kubernetes-dashboard:/proxy/

kubectl create serviceaccount dashboard-admin-sa

kubectl create clusterrolebinding dashboard-admin-sa \
  --clusterrole=cluster-admin \
  --serviceaccount=default:dashboard-admin-sa

kubectl get secrets

kubectl describe secret dashboard-admin-sa-token-wccdm

eyJhbGciOiJSUzI1NiIsImtpZCI6IlM1SlNNeE5BZXRQaDBQakxwZ092M0U2cVFUdkItTEVzOUtDQ1c2MFd0MU0ifQ.eyJpc3MiOiJrdWJlcm5ldGVzL3NlcnZpY2VhY2NvdW50Iiwia3ViZXJuZXRlcy5pby9zZXJ2aWNlYWNjb3VudC9uYW1lc3BhY2UiOiJkZWZhdWx0Iiwia3ViZXJuZXRlcy5pby9zZXJ2aWNlYWNjb3VudC9zZWNyZXQubmFtZSI6ImRhc2hib2FyZC1hZG1pbi1zYS10b2tlbi13Y2NkbSIsImt1YmVybmV0ZXMuaW8vc2VydmljZWFjY291bnQvc2VydmljZS1hY2NvdW50Lm5hbWUiOiJkYXNoYm9hcmQtYWRtaW4tc2EiLCJrdWJlcm5ldGVzLmlvL3NlcnZpY2VhY2NvdW50L3NlcnZpY2UtYWNjb3VudC51aWQiOiJmOGNlMjg5MC0yODQ3LTRhMDgtYjljMC00NDYxYWJkMTQ0OTYiLCJzdWIiOiJzeXN0ZW06c2VydmljZWFjY291bnQ6ZGVmYXVsdDpkYXNoYm9hcmQtYWRtaW4tc2EifQ.Nbs7p_8p381jOnR1haTGNP7LfiQBzZyoNRnimLaq8wu7z_F0rok2WycTd8fcMwnh27iZx5mDNnJrnmZeqONogY1MKtLpLZg-TZzkWZDZQetij2xX_7ONXMxoF8TaUvzjdHNks3y0AmfjvDJe2B3VARY4vmd14qcvKsDU4PvwfF8eNydYkX63pdAQzeLQTWZw3sNegQLDzUbsrQakX5k37Odvz5csrBbEnLEA3_ZttUqHumueVmMYtbVHvcKR_6cF_Iql6EkF_uEkCatvSm5kg9YXZVOgWSxt_rLgZG8MSENphQC4JIHixeCSaETJftHwkx4gaNxCH5kPIPSAQnYkETBA12s382rJnqzj9bNZ4AmfDLiM0NCIjVWVSiQoGO18aYH1jiyaw-1HanH4p5j3zdc03gnlYSljuMRwLz_3KYgEKpB3dXCAb-HAaw4MH-fPIAhBpMYXYBrGXJYjiSiCRdjBAU1z_jK5tJg6BZZXqi7BgfH4vArWTrItyIl-YawLeUcJ8w1KoTQvv84DCwoopBo1L6a2PfEdWxxfURsfQuoIIz0-ZJHXsjq2gy7-qdY8JF_WSo_wN-Y3oNRcv4fv1r9fJUwBFr_V7r-63A4WloyUXPTm5Yw4P1ukMREGbhkzo22wizG9kccTwab34zr2Eob-nKNjBsO30suaVxOnqYU


```