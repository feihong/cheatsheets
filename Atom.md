# Atom

## Turn off Welcome tabs

Uncheck "Show Welcome Guide when opening Atom"

## Opening `~/.atom/snippets.cson`:

### Mac

From the menu, select Atom > Open your snippets.

### Linux

From the menu, select Edit > Snippets...

## Show ignored files

1. Go to preferences and select packages.
1. Search for treeview.
1. Select settings for treeview.
1. Unselect `Hide VCS ignored files`.

## Snippets

```cson
'.source.python':
  'ipdb':
    'prefix': 'pdb'
    'body': 'import ipdb; ipdb.set_trace()'
  'ipython':
    'prefix': 'ipython'
    'body': 'import IPython; IPython.embed()'
  
'.source.js':
  'console.log':
    'prefix': 'log'
    'body': 'console.log($1)$2'

```
