## Konflikt opercji merge

Anulowanie operacji:
```bash
> git merge --abort
```

Jeżeli decydujemy się na rozwiązanie to dostajemy pliki z sekcjami mówiącymi z którego brancha pochodzą jakie zmiany. Ręcznie usuwamy zmiany które nam nie pasują oraz nagłówki gita. Bardzo łatwo robi się to w edytorach z wtyczkami, np. *VS Code*.

Po zakończeniu robimy:
```bash
> git add .
> commit -m "merge conflict resolved"
```