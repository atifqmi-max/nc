# nc - Blueprint Files

Is repo mein 2 blueprint files hain:

- `mcplugins.blueprint`
- `nebula.blueprint`

## VPS par Install / Download karne ka Tareeqa

In dono blueprint files ko `/var/www/pterodactyl` directory ke ander download karne ke liye, apne VPS ke terminal (SSH ya sshx) mein neeche wala command paste karo:

```bash
mkdir -p /var/www/pterodactyl && cd /var/www/pterodactyl && wget https://raw.githubusercontent.com/atifqmi-max/nc/main/mcplugins.blueprint && wget https://raw.githubusercontent.com/atifqmi-max/nc/main/nebula.blueprint && ls -la
```

### Ye command kya karta hai:

1. `mkdir -p /var/www/pterodactyl` — Agar ye directory maujood nahi hai to bana deta hai (agar pehle se hai to kuch nahi hota)
2. `cd /var/www/pterodactyl` — Usi directory mein chala jata hai
3. `wget .../mcplugins.blueprint` — GitHub se `mcplugins.blueprint` file download karta hai
4. `wget .../nebula.blueprint` — GitHub se `nebula.blueprint` file download karta hai
5. `ls -la` — Directory ke andar sab files/folders dikhata hai (confirm karne ke liye ke dono files sahi tarah aa gayi)

## Files Kahan Milengi?

Download hone ke baad dono blueprint files seedha `/var/www/pterodactyl/` folder ke andar milengi.

Check karne ke liye:

```bash
cd /var/www/pterodactyl
ls -la
```

## Repo Link

https://github.com/atifqmi-max/nc
