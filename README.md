# Описание файла gitignore для terraform
## Будут игнорироваться следующие файлы и директории:
1. Локальные директории .terraform
2. Файлы имеющие разрешение *.tfstate, *.tfstate.*, *.tfvars, *.tfvars.json
3. Файлы логирования crash.log, crash.*.log
4. Файлы override.tf, override.tf.json, *_override.tf, *_override.tf.json
5. Файлы конфигурации CLI .terraformrc, terraform.rc