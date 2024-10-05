# Conversion de Chaîne Hexadécimale en Texte

Ce script Python convertit une chaîne hexadécimale en texte lisible.

## Description

Le code source prend une chaîne de caractères représentant des valeurs hexadécimales, les convertit en bytes, puis décode ces bytes en une chaîne de caractères UTF-8.

## Code source

```python
# Hexadecimal string
hex_string = "63727970746f7b596f755f77696c6c5f62655f776f726b696e675f776974685f6865785f737472696e67735f615f6c6f747d"

# Convert the hex string to bytes
byte_array = bytes.fromhex(hex_string)

# Decode the bytes to a string
flag = byte_array.decode('utf-8')

# Print the flag
print(flag)
```

## Fonctionnement

1. **Définition de la chaîne hexadécimale** :
   - `hex_string` est une chaîne de caractères représentant des valeurs hexadécimales.

2. **Conversion en bytes** :
   - `byte_array = bytes.fromhex(hex_string)` convertit la chaîne hexadécimale en un tableau de bytes.

3. **Décodage en texte** :
   - `flag = byte_array.decode('utf-8')` décode le tableau de bytes en une chaîne de caractères UTF-8.

4. **Affichage du résultat** :
   - `print(flag)` affiche la chaîne de caractères obtenue.

## Utilisation

Pour utiliser ce script :

1. Assurez-vous d'avoir Python installé sur votre système.
2. Copiez le code dans un fichier `.py` (par exemple, `hex_converter.py`).
3. Exécutez le script en utilisant la commande : `python hex_converter.py`
4. Le résultat sera affiché dans la console.

## Note

Ce code semble être utilisé pour décoder un "flag" encodé en hexadécimal, probablement dans le contexte d'un défi de cryptographie ou de sécurité informatique.
