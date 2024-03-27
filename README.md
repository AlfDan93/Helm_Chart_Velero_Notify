# Helm Chart Velero Notify

1. Scarica il repo:
```
git clone https://github.com/AlfDan93/Helm_Chart_Velero_Notify.git
```
2. Entrare nella folder del repo git:
```
cd Helm_Chart_Velero_Notify
```
3. Installa Repo con helm lanciando il comando:
```
helm upgrade --install \ 
velero-backup-notify \
-n velero \
--set email.enabled=true \
--set email.failures_only=false \
--set email.smtp.host=... \
--set email.smtp.port=25 \
--set email.smtp.username=... \
--set email.smtp.password=... \
--set email.from_address=... \
--set email.to_address=... \
.
```
