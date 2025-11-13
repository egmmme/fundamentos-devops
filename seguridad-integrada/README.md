# 🔒 Seguridad Integrada (Shift-Left)
Incorporar seguridad desde las primeras fases del ciclo de vida del software.

## Mi Experiencia

### 1. **SAST en Pipeline**
```yaml
- name: Security Scan
  uses: sonarsource/sonarqube-scan-action@v1
  with:
    args: >
      -Dsonar.projectKey=my-project
```

### 2. **Dependency Scanning**
```bash
# npm audit en CI
npm audit --audit-level moderate
```

### 3. **Secret Management**
```yaml
# GitHub Secrets usage
env:
  DATABASE_URL: ${{ secrets.DATABASE_URL }}
  API_KEY: ${{ secrets.API_KEY }}
```

### 4. **Prácticas de Seguridad**
- ✅ Security reviews en PRs
- ✅ Escaneo automatizado de vulnerabilidades
- ✅ Verificaciones de seguridad de infraestructura
- ✅ Web Security Firewalls
