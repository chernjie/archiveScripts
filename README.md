archiveScripts
==============

A bash script that stores a log of single-line archived bash scripts (to itself), useful when "```Ctrl+R```", "```!```", ```alias```es and "```history```" do not solve your command line convenience


Example usage:
--------------

```
Usage: archiveScripts <script_number> [-n|--dry-run]
Usage: archiveScripts add <script>
Usage: archiveScripts edit|-e|help|-h|?
Usage: archiveScripts <regex> [-r|-R|run]
```

```bash
$ archiveScripts add 'echo a single line command line that you want to archive #randomnamedkey'

$ archiveScripts 32 -n
echo a single line command line that you want to archive #randomnamedkey

$ archiveScripts 32
a single line command line that you want to archive #randomnamedkey

$ archiveScripts randomnamedkey -r
echo a single line command line that you want to archive #randomnamedkey
a single line command line that you want to archive #randomnamedkey

$ archiveScripts randomnamedkey -R
a single line command line that you want to archive #randomnamedkey

```

Alternatives:
http://www.logicalpoetry.com/bashalias/