# Installeer als AppImage

U kunt de nieuwste AppImage downloaden van de [QOwnNotes-releasepagina](https://github.com/pbek/QOwnNotes/releases). Het zou op die pagina de naam `QOwnNotes-x86_64.AppImage` moeten hebben.

::: tip
Als je [jq](https://stedolan.github.io/jq/) hebt geïnstalleerd, kun je ook download de nieuwste AppImage direct:

```bash
# query the latest Linux release from the QOwnNotes API, parse the JSON for the URL and download it
curl -L https://api.qownnotes.org/latest_releases/linux | jq .url | xargs curl -Lo QOwnNotes-x86_64.AppImage
```
:::

Vervolgens kunt u de uitvoeringsrechten voor het bestand wijzigen:

```bash
chmod a+x QOwnNotes-*.AppImage
```

Daarna zou u de AppImage moeten kunnen uitvoeren om QOwnNotes uit te voeren.

::: warning
If you want to use the **automatic updater** please make sure to put your AppImage in a place where your user account has write-access to, like somewhere in your home directory.
:::
