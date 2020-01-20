**Description (Описание)**
<p>This integration allows you to display the history of today's movements on the map of your HomeAssistant (Интеграция позволяет отображать историю сегодняшних перемещений на карте в вашем HomeAssistant)</p>

**Example configuration.yaml:**

```yaml
sensor:
  platform: route
  name: route
  haddr: 'https://your_ha_address.com'
  entityid: ha_entity_id_you_want_to_watch
  timezone: '+02:00'
  token: 'your_generated_long_life_token_ha_api'
```

**Configuration variables:**  
  
key | description  
:--- | :---  
**platform (Required)** | The platform name (имя платформы)
**name (Option)** | The name of this element in HA interface (имя элемента в интерфейсе HA)
**haddr (Required)** | base_url of HA (base_url вашего HA)
**entityid (Required)** | the HA entityid of your device_tracker (это ID вашего устройства, за которым будете наблюдать)
**timezone (Required)** | is your timezone, for example '+03:00' (ваш часовой пояс, например '+03:00')
**token (Required)** | the access token previously received in the frontend of HomeAssistant to use REST API (предварительно полученный во фронтенде HomeAssistant токен доступа для использования REST API)
  
