# Lovesmen.gay Subdomain system
This is a registry for free subdomains on the domain lovesmen.gay.

## How to use 
1. Fork this repo
2. Make a JSON file in domains, the name of the json being how you would like to call the subdomain (for example, if you want arty.lovesmen.gay, you would need to call the JSON arty.json)
3. Make a json file like so:
```
{
    "owner": {
        "username": "MrArtyH"
    },

    "record": {
        "MX": ["mail.protonmail.ch", "mailsec.protonmail.ch"],
        "TXT": ["protonmail-verification=8dbc9639530d0f12b7ff3830b4a7ddd58b535498", "v=spf1 include:_spf.protonmail.ch ~all"]
    }
}
```
You can use many records, such as MX, TXT, CNAME, A and AAAA, including many others.
4. Send a pull request with the newly added JSON file
5. Wait until it gets accepted and you're done!

## Credits to iostpa for making the setup :3 
