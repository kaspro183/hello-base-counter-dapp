
# Hello Base – Counter dApp (sans terminal)

Ce repo contient un **smart contract Counter** et une **interface web simple (HTML/JS)** pour interagir avec lui sur **Base Sepolia (testnet)**, sans outils de build.

## Structure
```
contracts/Counter.sol      # Contrat Solidity
frontend/index.html        # dApp web (ethers via CDN)
abi/Counter.json           # ABI du contrat
```

## Déployer le contrat (Remix, sans terminal)
1. Ouvre https://remix.ethereum.org
2. Crée un fichier `Counter.sol` et colle le contenu de `contracts/Counter.sol`.
3. Compile avec `0.8.20` (ou compatible).
4. Dans MetaMask, ajoute le réseau **Base Sepolia** (Chain ID `84532`).
5. Dans Remix, sélectionne l'environnement **Injected Provider - MetaMask** (ça utilisera Base Sepolia).
6. Déploie le contrat `Counter`. Copie **l'adresse déployée**.

## Utiliser la dApp (local file ou GitHub Pages)
- Ouvre `frontend/index.html` dans ton navigateur **avec MetaMask installé**.
- Colle l'adresse du contrat dans le champ prévu, clic **Charger ABI & Contrat**.
- Utilise **Lire** et **increment()** pour voir/mettre à jour le compteur.

> Tu peux aussi héberger `frontend/` via GitHub Pages : Settings → Pages → Branche `main` → dossier `/root` (ou `/frontend` selon ton layout).

## Pousser sur GitHub (sans terminal)
1. Crée un nouveau repo sur GitHub.
2. Clique **Add file → Upload files** et glisse le contenu de ce projet.
3. Écris un message de commit (ex: "feat: hello base counter dapp") et valide.
4. (Optionnel) Active **GitHub Pages** pour publier l'UI.

## Talent Protocol
- Assure-toi d'avoir relié GitHub dans ton profil Talent Protocol.
- Après le commit, va sur Talent Protocol → **Sync GitHub** pour rafraîchir tes contributions.

## Licence
MIT
