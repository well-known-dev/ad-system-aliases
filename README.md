# ad-system-aliases
A community registry of programmatic ad system domain aliases.

AdTech standards like [ads.txt](https://iabtechlab.com/ads.txt/),
[sellers.json](https://iabtechlab.com/sellers-json/), and
[SupplyChain Object](https://github.com/InteractiveAdvertisingBureau/openrtb/blob/master/supplychainobject.md)
identify SSPs, ad exchanges, and other AdTech companies by their "Ad System Domains".

However, these companies often change their names and domains due to mergers, rebranding, etc., or
even operate from multiple domains at the same time. It can be hard to keep track of what domain to
use at any given time, and what domains actually refer to the same ad system.

This project aims to maintain a list of ad system domain aliases and the main ad system domain that
should be used instead. This list is available in CSV format:
[ad_system_aliases.csv](/ad_system_aliases.csv).

As this is a community project, these mappings are educated guesses based on available information.
They may not be correct, so use at your own risk. If you have a correction or addition, please
[raise an issue](https://github.com/well-known-dev/ad-system-aliases/issues).

## Notes:
- This project tracks ad system domains used in standards, not company websites or names, or ad
  system ownership. Companies may have multiple ad systems domains for different ad systems they
  run, and the current main ad system domain may not match the current website/name/branding for the
  ad system or company.
- This project doesn't list all ad system domains - only alias ad system domains.
- To be considered an ad system domain, a domain typically needs to host a sellers.json file, and
  be referenced in at least one ads.txt or app-ads.txt file.
- Two ad system domains are considered to refer to the same ad system if they have the same
  sellers.json - either exactly the same file, or with the same sellers listed.
- Baring other information, the main ad system domain is typically assumed to be the one referenced
  most often in ads.txt and app-ads.txt files.
