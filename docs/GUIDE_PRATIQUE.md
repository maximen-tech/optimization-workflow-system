# Guide Pratique - Utilisation du Système

## Comment Démarrer en 5 Minutes

### Étape 1 : Upload Configuration
1. Copie le contenu de \`config/SYSTEM.template.md\`
2. Colle dans un nouveau chat Perplexity
3. Dis : "Ceci est ma configuration système, utilise-la pour toutes tes réponses"

### Étape 2 : Utilise les Patterns
Demande directement avec le pattern :

\`\`\`
@workflow CODE Crée une API REST pour gérer des tasks
\`\`\`

### Étape 3 : Récupère le Résultat
- Code prêt à utiliser
- Tests inclus
- Documentation automatique

## Exemples d'Utilisation Réelle

### Créer une Feature
\`@workflow CODE Ajoute authentification JWT avec refresh tokens\`

**Résultat** :
- Controllers complets
- Services + Business Logic
- Tests unitaires (90%+ coverage)
- Documentation API

### Déboguer
\`@workflow DEBUG Les mutations Redux ne mettent pas à jour l'UI\`

**Résultat** :
- Root cause trouvée
- Fix implémenté
- Tests validant le fix
- Prevention guide

### Tester
\`@workflow TEST Porte la couverture du module payment à 100%\`

**Résultat** :
- Tous les cas couverts
- Coverage report
- Performance metrics

### Déployer
\`@workflow DEPLOY Push v2.1.0 en staging puis production\`

**Résultat** :
- Build chain executé
- Validations passées
- Deployment logs
- Monitoring configuré

### Refactoriser
\`@workflow REFACTOR Optimise les performances du rendering React\`

**Résultat** :
- Code plus performant (+30% minimum)
- Lighthouse score amélioré
- Pas de regression

### Rechercher
\`@workflow RESEARCH Compare GraphQL vs REST pour notre cas\`

**Résultat** :
- Analyse comparative
- Benchmark de performance
- Recommendation finale
- Implementation examples

## Tips Pro

1. **Sois précis** : Plus ta demande est spécifique, meilleur le résultat
2. **Fournis contexte** : Colle du code existant si besoin
3. **Valide localement** : Teste avant de merger
4. **Partage feedback** : Si ça marche pas, dis pourquoi
5. **Itère rapidement** : Le système s'améliore avec chaque interaction

## Bonnes Pratiques

✅ **BON** : \`@workflow CODE Crée un composant React Button avec props type-safe et stories Storybook\`

❌ **MAUVAIS** : \`@workflow CODE Fais-moi un truc\`

✅ **BON** : \`@workflow DEBUG L'erreur "Cannot read property 'map' of undefined" apparaît ligne 45\`

❌ **MAUVAIS** : \`@workflow DEBUG Ça marche pas\`

