# 🤖 Rotinas e Automações

### Iluminação

#### Exemplo: Acender Luz ao Anoitecer

```yaml
automation:
  - alias: Acender luz da sala ao anoitecer
    trigger:
      platform: sun
      event: sunset
    action:
      service: light.turn_on
      target:
        entity_id: light.living_room_ceiling_light
```