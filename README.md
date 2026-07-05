# nc - Blueprint Files

Is repo mein `nc-main.zip` file hai jis ke andar blueprint files hain.

## VPS par Install / Download karne ka Tareeqa

Blueprint files ko `/var/www/pterodactyl` directory ke ander install karne ke liye, apne VPS ke terminal (SSH ya sshx) mein neeche wala command paste karo:

```bash
mkdir -p /var/www/pterodactyl && cd /var/www/pterodactyl && wget https://raw.githubusercontent.com/atifqmi-max/nc/main/nc-main.zip && unzip -o nc-main.zip && rm nc-main.zip && ls -la
```

### Ye command kya karta hai:

1. `mkdir -p /var/www/pterodactyl` — Agar ye directory maujood nahi hai to bana deta hai (agar pehle se hai to kuch nahi hota)
2. `cd /var/www/pterodactyl` — Usi directory mein chala jata hai
3. `wget ...` — GitHub se `nc-main.zip` file download karta hai
4. `unzip -o nc-main.zip` — Zip file ko seedha `/var/www/pterodactyl` ke andar hi extract kar deta hai (blueprint files yahin mix ho jati hain)
5. `rm nc-main.zip` — Download hui zip file delete kar deta hai (space bachane ke liye)
6. `ls -la` — Directory ke andar sab files/folders dikhata hai (confirm karne ke liye ke sahi tarah extract hui)

## Agar `unzip` install nahi hai

Pehle ye command chalao:

```bash
apt update && apt install -y unzip
```

Uske baad upar wala main command dobara chalao.

## Files Extracted Kahan Milengi?

Extract hone ke baad blueprint files seedha `/var/www/pterodactyl/` folder ke andar milengi (koi alag sub-folder nahi banega).

Check karne ke liye:

```bash
cd /var/www/pterodactyl
ls -la
```

## Repo Link

https://github.com/atifqmi-max/nc
