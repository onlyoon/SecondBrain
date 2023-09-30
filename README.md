
---
cssclass: dashboard

---

# [](https://github.com/TfTHacker/DashboardPlusPlus/blob/master/Dashboard%2B%2B.md#personal-projects)Areas Of Responsibility

##### 📌 Index
- 💻 Dev
    - [[Algorithm & DataStructure]]
    - [[React]]
    - [[JavaScript]]
    - [[Svelte]]
    - [[CSS]]
    - [[Blender]]
- Blockchain
	- Ethereum

# [](https://github.com/TfTHacker/DashboardPlusPlus/blob/master/Dashboard%2B%2B.md#vault-info)Vault Info

- 🗄️ Recent file updates `$=dv.list(dv.pages('').sort(f=>f.file.mtime.ts,"desc").limit(10).file.link)`
- 🔖 Tagged: favorite `$=dv.list(dv.pages('#favorite').sort(f=>f.file.name,"desc").limit(4).file.link)`
- 〽️ Stats
    - File Count: `$=dv.pages().length`
    - Personal recipes: `$=dv.pages('"Family/Recipes"').length`