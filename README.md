# Scanner User Agents

The idea of this project is to collect a list of user agent strings used by common web application scanners, things like [Nikto](https://github.com/sullo/nikto) or Acunetix. These strings can then be used by defenders to block or play with attackers.

I've no idea what the best format for this is so I'm going to start with a very simple JSON object and see what happens.

```json
{
  "ua": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/74.0.3729.169 Safari/537.36",
  "scanner": "Nikto",
  "version": "Github master branch",
  "last seen": "2022-06-23"
}
```

If you think this could be improved, please make suggestions sooner rather than later, I'd rather mess with the format at the start than in six months.

The idea is based on a [short Twitter chat](https://twitter.com/dcuthbert/status/1539894585811505152) with [Daniel Cuthbert](https://github.com/danielcuthbert).
