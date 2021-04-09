# naarivad.py

A discord.py compatible extension for the Naarivad discord server.

## Prerequisites

- discord.py>=1.5
- asyncpg>=0.21.0
- psql>=11
- A subclass of [`commands.Bot`](https://discordpy.readthedocs.io/en/latest/ext/commands/api.html#discord.ext.commands.Bot)
  that implements a `pool` attribute, which is an instance of [`asyncpg.Pool`](https://magicstack.github.io/asyncpg/current/api/index.html#asyncpg.pool.Pool).
  
## Before running
In your psql tool, after connecting to your database, run the following:
```sql
CREATE TABLE IF NOT EXISTS naarivad_posts (
    id TEXT,
    translated_into VARCHAR(3) ARRAY,
    PRIMARY KEY (id)
);
```

To make this easier, there are commented out lines that define this table using a pseudo-ORM, which can be taken from my other project [here](https://github.com/darthshittious/Robo-VJ/blob/main/cogs/utils/db.py)

## Running

Just clone this (into a cogs/extensions directory maybe) and load the `naarivad` extension.

## Troubleshooting

You should ideally not run into trouble here. You should be comfortable with using discord.py, or at least willing to read the documentation and figure stuff out. 

Don't create issues that aren't directly caused by the code in this repository.
