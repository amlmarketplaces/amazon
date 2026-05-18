# amlmarketplaces/amazon

Claude Code marketplace federating all `@amlplugins/amazon-*` plugins.

## Install

Add to your project's `.claude/settings.json`:

```json
{
  "extraKnownMarketplaces": {
    "aml-amazon": {
      "source": { "source": "github", "repo": "amlmarketplaces/amazon" }
    }
  },
  "enabledPlugins": {
      "amazon-bedrock@aml-amazon": true,
      "amazon-cloudfront@aml-amazon": true,
      "amazon-cognito@aml-amazon": true,
      "amazon-comprehend@aml-amazon": true,
      "amazon-dynamodb@aml-amazon": true
    }
}
```

Then launch Claude Code in the project. The marketplace is fetched from `amlmarketplaces/amazon`, cached under `~/.claude/plugins/cache/aml-amazon/`, and each enabled plugin is loaded from its `amlplugins` source repo.

## Plugins (15 total)

- `amazon-bedrock` — [@amlplugins/amazon-bedrock](https://github.com/amlplugins/amazon-bedrock)
- `amazon-cloudfront` — [@amlplugins/amazon-cloudfront](https://github.com/amlplugins/amazon-cloudfront)
- `amazon-cognito` — [@amlplugins/amazon-cognito](https://github.com/amlplugins/amazon-cognito)
- `amazon-comprehend` — [@amlplugins/amazon-comprehend](https://github.com/amlplugins/amazon-comprehend)
- `amazon-dynamodb` — [@amlplugins/amazon-dynamodb](https://github.com/amlplugins/amazon-dynamodb)
- `amazon-ec2` — [@amlplugins/amazon-ec2](https://github.com/amlplugins/amazon-ec2)
- `amazon-ecs` — [@amlplugins/amazon-ecs](https://github.com/amlplugins/amazon-ecs)
- `amazon-lambda` — [@amlplugins/amazon-lambda](https://github.com/amlplugins/amazon-lambda)
- `amazon-polly` — [@amlplugins/amazon-polly](https://github.com/amlplugins/amazon-polly)
- `amazon-rds` — [@amlplugins/amazon-rds](https://github.com/amlplugins/amazon-rds)
- `amazon-rekognition` — [@amlplugins/amazon-rekognition](https://github.com/amlplugins/amazon-rekognition)
- `amazon-s3` — [@amlplugins/amazon-s3](https://github.com/amlplugins/amazon-s3)
- `amazon-ses` — [@amlplugins/amazon-ses](https://github.com/amlplugins/amazon-ses)
- `amazon-sns` — [@amlplugins/amazon-sns](https://github.com/amlplugins/amazon-sns)
- `amazon-sqs` — [@amlplugins/amazon-sqs](https://github.com/amlplugins/amazon-sqs)

## Related

- npm packages: `@amlplugins/amazon-*` published to GitHub Packages (`https://npm.pkg.github.com`).
- Aggregating parent: [`amlmarketplaces/aml`](https://github.com/amlmarketplaces/aml) — federates every `@amlplugins/*` plugin under a single marketplace.
- AML topology: see `.claude/rules/definitions/ageni.md` § "GitHub Topology" — this repository is a Tier-4 HUB-INSTANCE under the `amlmarketplaces/` Tier-3 HUB-ORGANIZATION.

> Built by `.claude/skills/aml/metateam/marketplace/test/cross-org-amlmarketplaces-batch.mjs`.
