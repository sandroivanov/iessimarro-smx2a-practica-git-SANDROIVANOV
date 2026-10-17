### Descrpicio dels pasos seguits: Configuracio del servei DHCP 

En aquesta seccio es detallem els passos realitzats per a la posada en marxa i configuracio del servei DHCP a l'aula digital, seguint les indicacion de l'Annex B.

* **1. Activacio del servei DHCP**

- Instalacio del paquet corresponent al servidor DHCP.
- Activacio i habilitacio del server perque s'inici de manera automaticament amb el sistema.

* **2. Configuracio del rang d'adreces:**

- Edicio del fitxer de configuracio del DHCP per establir el rang d'IPs assignades automaticament als equips clients de l'aula:
  * **Rang establert** `192.168.1.10` a `192.168.1.50`.
  * **Mascara de subxarxa:** `255.255.255.0`.

* **3. Porta d'enllaç i servidor DNS** 
- Configuracio dels parametres de xaexa addicionals que s'envien automaticament als clients:
  * **Porta d'enllaç (Gateway)** `192.168.1.1`
  * **Servidor DNS** `8.8.8.8` / `1.1.1.1`

* **4. Verificacio amb tres equips de prova**
- Connexio de tres equips de prova diferents a la xarxa de l'aula.
- Comprovacio mitjançant la comanda `ipconfig` que cada equip rep correctament una IP dins del rang definit.
-Verificacio de la connectivitat fent un `ping` cap a la porta d'enllaç i a Internet del tres equips
