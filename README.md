# Lovesmen.gay Subdomain system
This is a registry for free subdomains on the domain lovesmen.gay.

## How to use 
1. Fork this repo
2. Make a JSON file in domains, the name of the json being how you would like to call the subdomain (for example, if you want arty.lovesmen.gay, you would need to call the JSON arty.json)
3. Make a JSON file like so:
```
{
    "owner": {
        "username": "your-github-username"
    },

    "record": {
        "A": ["1.1.1.1", "1.0.0.1"],
        "AAAA": ["2606:4700:4700::1111", "2606:4700:4700::1001"],
        "CNAME": "example.com",
        "MX": ["mx1.example.com", "mx2.example.com"],
        "TXT": ["example_verification=1234567890"],
        "NS": ["ns1.example.com", "ns2.example.com"],
        "SRV": [
            { "priority": 10, "weight": 60, "port": 5060, "target": "sipserver.example.com" },
            { "priority": 20, "weight": 10, "port": 5061, "target": "sipbackup.example.com" }
        ]
    }
}
```
You can use many records, such as MX, TXT, CNAME, A and AAAA, including many others.
You can also add other records.

4. Send a pull request with the newly added JSON file
5. Wait until it gets accepted and you're done!

## Credits to iostpa for making the setup :3 
