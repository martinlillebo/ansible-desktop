# ansible-desktop
Ansible-config av desktopen min, vanligvis Debian/GNOME3

Kan modifiseres av andre som vil sikre sin egen maskinconfig. til den dagen man skal eller må bytte personlig datamaskin

- Forberedelser før kjøring: 
    - Opprett en `inventory-ini` med riktig maskinreferanse
    - Kommenter vekk ev. uinteressante roles
    - Test gjerne på en VM først for å sikre at alt blir som du ønsker, før du prøver deg på en ekte datamaskin hvor det ikke fins noen angreknapp

- Kjøres slik: 
    - `ansible-playbook -i inventory.ini playbook.yml --diff`

## Hvis du ikke er meg, bør du gjøre dette først:

- Kommenter vekk alle role-ene i lista nedenfor. Disse er enten knyttet opp mot private repos jeg har, eller er sannsynligvis uinteressante for de fleste andre 
    - autokey-config
    - clone-ansible-desktop
    - clone-dotfiler
    - clone-notater
    - keyd-innstallering
    - subliemeless-desktop
    - zsh-omz

- Se gjennom `terminalprogrammer`-rollen og kommenter vekk uinteressante programmer
- ...se gjennom alt annet også :) 
