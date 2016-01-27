Open `~/.atom/snippets.cson`:

From the menu, select Atom > Open your snippets.

## Snippets

```cson
'.source.python':
  'pdb':
    'prefix': 'pdb'
    'body': 'import ipdb; ipdb.set_trace()'
    
'.source.python':
  'ipython':
    'prefix': 'ipython'
    'body': 'import IPython; IPython.embed()'
```
