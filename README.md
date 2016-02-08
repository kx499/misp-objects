# misp-objects

MISP objects to be used in MISP (3.0) system and can be used by other information sharing tool

~~~~json
{
        "name": "domain|ip",
        "meta-category": "network",
        "description": "A domain and IP address seen as a tuple in a specific time frame.",
        "version": 1,
        "attributes" :
        {
                "ip": {
                        "misp-object": "ip-dst",
                        "misp-usage-frequency": 1,
                        "categories": ["Network activity","External analysis"]
                },
                "domain": {
                        "misp-object": "domain",
                        "misp-usage-frequency": 1,
                        "categories": ["Network activity","External analysis"]
                },
                "first-seen": {
                        "misp-object": "datetime",
                        "misp-usage-frequency": 0
                },
                "last-seen": {
                        "misp-object": "datetime",
                        "misp-usage-frequency": 0
                }

        },
        "required": ["ip","domain"]
}
~~~~