# 🚩 Challenge 1: 🔏 Decentralized Staking App

Esta fue el codigo que use para subir el desafio 1, la diferencia es :
Tuve que agregarle a la direccion que generada por yarn generate, mas o menos la cantidad de 0.01 Ether en la red sepolia

Utilice una API de Alchemy, la cual tuve que colocarla en los archivos:
packages>netjs>scaffold.config.ts (en la linea 23):

alchemyApiKey: process.env.NEXT_PUBLIC_ALCHEMY_API_KEY || "oKxs-03sij-U_N0iOlrSsZFr29-IqbuF", lo que viene despues del || es mi API Key de Alchemy.

Tambien lo edite en:

packages>hardhat>.env.example
en donde dice:
ALCHEMY_API_KEY= 
Luego cambie el nombre del archivo a .env.local

Y por ultimo lo edite en:
packages>nextjs>.env.example
en donde dice:
NEXT_PUBLIC_ALCHEMY_API_KEY=
Luego cambie el nombre de este archivo nuevamente a .env.local

Para Obtener la API de Alchemy simplemente te logeas:

vas a App y crear una nueva App (en caso que no la tengas creada).
Luego en la esquina superior derecha aparece API_KEY, esa es la que se copia
