# naarivad.py

A discord.py compatible extension for the Naarivad discord server.

## Prerequisites

- discord.py>=1.5
- A subclass of [`commands.Bot`](https://discordpy.readthedocs.io/en/latest/ext/commands/api.html#discord.ext.commands.Bot)
  `session` attribute, which is an instance of [`iohttp.ClientSession`](https://docs.aiohttp.org/en/stable/client_reference.html#aiohttp.ClientSession).
- Access tokens to authenticate your uploads and post updates with the website. 
  (in this module, they are referenced as `bot.config.naarivad_upload_token`and `bot.config.naarivad_backend_token`. Edit this as necessary.)

## Running

Just clone this (into a cogs/extensions directory maybe) and load the `naarivad` extension.

## Troubleshooting

You should ideally not run into trouble here. You should be comfortable with using discord.py, or at least willing to read the documentation and figure stuff out. 

This module also isn't really portable and has no use outside of this. However, since I already released it along with my other bot, I have decided to keep it open source.

Don't create issues that aren't directly caused by the code in this repository.
