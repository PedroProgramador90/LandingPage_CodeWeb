# Clone o repositório
git clone https://github.com/PedroProgramador90/Insure_landing_page.git
cd Insure_landing_page

# Mova todos os arquivos para a raiz
mv Insure_landing_page/* .
mv Insure_landing_page/.* . 2>/dev/null  # Move arquivos ocultos se existirem

# Remove a pasta vazia
rmdir Insure_landing_page

# Commit e push
git add .
git commit -m "fix: move files to root directory"
git push origin main
```

### **Opção 3: Configurar a Vercel para a subpasta** ⚙️

Se preferir manter a estrutura atual:

1. Vá em **Settings** do projeto na Vercel
2. Em **Root Directory** → coloque: `Insure_landing_page`
3. Clique em **Save**
4. Vá em **Deployments** → clique nos `...` → **Redeploy**

---

## 🎯 Estrutura Correta (Recomendada)

Depois da correção, seu repo deve ficar assim:
```
Insure_landing_page/  (repositório)
├── index.html        ← Na raiz!
├── style.css
├── script.js
├── images/
├── design/
└── README.md
