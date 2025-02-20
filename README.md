# Kubernetes Terraform Setup

Dieses Projekt bietet ein Terraform-Setup zur Bereitstellung eines Kubernetes-Clusters mit einem Nginx-Deployment und einem Service.

## 🛠 Anforderungen
- **Terraform** (https://developer.hashicorp.com/terraform/downloads)
- **Kubernetes** (https://kubernetes.io/docs/tasks/tools/)
- **Minikube** (empfohlen für lokale Tests: https://minikube.sigs.k8s.io/docs/start/)

## 🚀 Installation & Nutzung

### 1️⃣ Minikube starten
```sh
minikube start
```

### 2️⃣ Terraform initialisieren
```sh
terraform init
```

### 3️⃣ Infrastruktur bereitstellen
```sh
terraform apply -auto-approve
```

### 4️⃣ Zugriff auf Nginx-Service erhalten
```sh
minikube service nginx-service --url
```
Der obige Befehl gibt eine URL aus, über die Nginx erreichbar ist.

## 📂 Projektstruktur
```
├── main.tf          # Terraform Konfiguration
├── README.md        # Dieses Dokument
└── .terraform/      # Terraform Abhängigkeiten (nach init)
```

## 🔄 Infrastruktur löschen
Falls du die erstellte Infrastruktur entfernen möchtest:
```sh
terraform destroy -auto-approve
```

## 📜 Lizenz
Dieses Projekt steht unter der MIT-Lizenz.

---
🎉 Viel Spaß mit Kubernetes und Terraform!

