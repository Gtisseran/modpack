# Attributions — Modpack Nations

Ce dépôt distribue le modpack du serveur Minecraft **Nations**
(Minecraft Java 1.20.1 · Forge 47.4.10).

## Mods

Les fichiers de `overrides/mods/` sont des mods qui ne sont pas hébergés sur
Modrinth. Ils sont redistribués ici conformément aux licences de leurs
auteurs respectifs.

| Mod | Version | Source | Licence |
| --- | --- | --- | --- |
| Create: Explosives | beta V0.1.7.15 | CurseForge | à vérifier auprès de l'auteur |
| GeckoLib | 4.8.4 | CurseForge / Modrinth | LGPL-3.0 |
| TerraBlender | 3.0.1.10 | CurseForge / Modrinth | LGPL-3.0 |
| Plasmo Voice Chat | 2.6.22 | CurseForge / Modrinth | MIT |

Les 26 autres mods du pack sont téléchargés directement depuis le CDN de
Modrinth par le launcher, à partir des empreintes SHA-512 du manifeste.
Leurs licences et attributions sont consultables sur la page de chaque
projet Modrinth.

## Manifeste

`manifest.json` est généré à partir du pack Modrinth d'origine :

```
node modpack/import-mrpack.mjs "<fichier>.mrpack"
```

Le launcher Nations lit ce manifeste, télécharge chaque fichier, vérifie son
empreinte, et supprime les mods qui ne font plus partie du pack.
