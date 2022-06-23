# Scanner User Agents

The idea of this project is to collect a list of user agent strings used by common web application scanners, things like [Nikto](https://github.com/sullo/nikto) or Acunetix. These strings can then be used by defenders to block or play with attackers.

I've no idea what the best format for this is so I'm going to start with a very simple JSON object and see what happens.

```json
{
  "ua": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/74.0.3729.169 Safari/537.36",
  "scanner": "Nikto",
  "version": "Github master branch",
  "last seen": "2022-06-23",
  "known ips": [
    "1.2.3.4",
	"2.3.4.5"
  ]
}
```

If you think this could be improved, please make suggestions sooner rather than later, I'd rather mess with the format at the start than in six months.

## Updates

At a suggestion from a viewer, I've just added known scanner IP addresses to the structure. It won't be much use for the majority of tools, but bigger vendors, such as Acunetix, publish their scanner IPs and so including these may be of use.

## Warning

Some of these scanners use the same UAs as legitimate browsers, for example Nikto, and so blindly blocking or messing with traffic based purely on items in this list could affect real users. Think before you use it.

The idea is based on a [short Twitter chat](https://twitter.com/dcuthbert/status/1539894585811505152) with [Daniel Cuthbert](https://github.com/danielcuthbert).
