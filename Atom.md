# Atom

## Opening `~/.atom/snippets.cson`:

### Mac

From the menu, select Atom > Open your snippets.

### Linux

From the menu, select Edit > Snippets...

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
