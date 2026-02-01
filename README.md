# Donut-SMP-Tab-Ve-Scoreboard-Kodlar- işte kod
animations.yml:

donut_header:
  enabled: true
  interval-ticks: 60
  messages:
  - <#00ADFC>&lPbfSMP</#00ADFC>
  - <#00ADFC>&lPbfSMP &7- &ePlay Now!</#00ADFC>
  - '&7Welcome &f%player% &7to &eDonut SMP'
  - '&7Join &b%server_ip%&7 - &f%server_online% players'
donut_footer:
  enabled: true
  interval-ticks: 80
  messages:
  - '   &#37BFF9/ᴅɪꜱᴄᴏʀᴅ  /ɢᴜɪᴅᴇ  /ꜱᴛᴏʀᴇ   '
  - '&7Discord: &bdiscord.gg/yourserver'
  - '&7Store: &bstore.pbf.net'
donut_sidebar:
  enabled: true
  interval-ticks: 50
  lines:
  - ''
  - <#00FC00>&l$</#00FC00> &fMoney <#00FC00>%vault_eco_balance_formatted%</#00FC00>
  - <#A303F9>★</#A303F9> &fShards
  - <#FC0000>🗡</#FC0000> &fKills <#FC0000>%statistic_player_kills%</#FC0000>
  - <#F97603>☠</#F97603> &fDeaths <#F97603>%statistic_deaths%</#F97603>
  - <#00A4FC>⌛</#00A4FC> &fKeyall <#00A4FC>%zschedulers_time_keyall%</#00A4FC>
  - <#FCE300>⌚</#FCE300> &fPlaytime <#FCE300>%statistic_hours_played%h %statistic_time_played:minutes%m</#FCE300>
  - ''
  - <#A8A8A8>NA East (<#00A4FC>%player_ping%</#00A4FC>)</#A8A8A8>
donut_tab_top:
  enabled: true
  interval-ticks: 70
  messages:
  - <#00ADFC>&lPbfSMP &7- &e%server_motd%</#00ADFC>
  - '&7Have fun &f%player%&7!'


şimdi buda config.yml

header-footer:
  enabled: true
  designs:
    world-world1:
      display-condition: '%world%=world1'
      header:
      - an example of world with custom
      footer:
      - header/footer and prefix/suffix
    world-world2;world3:
      display-condition: '%world%=world2|%world%=world3'
      header:
      - This is a shared header for
      - world2 and world3
      footer: []
    server-server1:
      display-condition: '%server%=server1'
      header:
      - an example of server with custom header
      footer: []
    default:
      display-condition: '%world%!=disabledworld'
      header:
      - ''
      - <#00ADFC>&lPbfSmp</#00ADFC>
      - '&f%server_online% Players'
      - ''
      footer:
      - ''
      - '   &#37BFF9/ᴅɪꜱᴄᴏʀᴅ  /ɢᴜɪᴅᴇ  /ꜱᴛᴏʀᴇ   '
      - ''
tablist-name-formatting:
  enabled: true
  disable-condition: '%world%=disabledworld'
scoreboard-teams:
  enabled: true
  enable-collision: true
  invisible-nametags: false
  sorting-types:
  - GROUPS:owner,admin,mod,helper,builder,vip,default
  - PLACEHOLDER_A_TO_Z:%player%
  case-sensitive-sorting: true
  can-see-friendly-invisibles: false
  disable-condition: '%world%=disabledworld'
playerlist-objective:
  enabled: true
  value: '%ping%'
  fancy-value: '&7Ping: %ping%'
  title: Java Edition is better
  render-type: INTEGER
  disable-condition: '%world%=disabledworld'
belowname-objective:
  enabled: false
  value: '%health%'
  title: '&cHealth'
  fancy-value: '&c%health%'
  fancy-value-default: NPC
  disable-condition: '%world%=disabledworld'
prevent-spectator-effect:
  enabled: false
bossbar:
  enabled: false
  toggle-command: /bossbar
  remember-toggle-choice: false
  hidden-by-default: false
  bars:
    ServerInfo:
      style: PROGRESS
      color: '%animation:barcolors%'
      progress: '100'
      text: '&fWebsite: &bwww.pbf.com'
scoreboard:
  enabled: true
  toggle-command: /sb
  remember-toggle-choice: false
  hidden-by-default: false
  delay-on-join-milliseconds: 0
  respect-other-plugins: true
  scoreboard:
  scoreboards:
    not-in-team:
      title: '  <#007CF9>&lPbfSMP</#007CF9>  '
      lines:
        - ''
        - '<#00FC00>$</#00FC00> &fMoney <#00FC00>%vault_eco_balance_formatted%</#00FC00>'
        - '<#A303F9>★</#A303F9> &fShards'
        - '<#FC0000>🗡</#FC0000> &fKills <#FC0000>%statistic_player_kills%</#FC0000>'
        - '<#F97603>☠</#F97603> &fDeaths <#F97603>%statistic_deaths%</#F97603>'
        - '<#00A4FC>⌛</#00A4FC> &fKeyall <#00A4FC>%zschedulers_time_keyall%</#00A4FC>'
        - '<#FCE300>⌚</#FCE300> &fPlaytime <#FCE300>%statistic_hours_played%h %statistic_time_played:minutes%m</#FCE300>'
        - ''
        - '<#A8A8A8>NA East (<#00A4FC>%player_ping%</#00A4FC>)</#A8A8A8>'

layout:
  enabled: false
  direction: COLUMNS
  default-skin: mineskin:383747683
  enable-remaining-players-text: true
  remaining-players-text: '... and %s more'
  empty-slot-ping-value: 1000
  layouts:
    default:
      fixed-slots:
      - '1|&3Website&f:'
      - 2|&bmyserver.net
      - '3|&8&m                       '
      - '4|&3Name&f:'
      - 5|&b%player%
      - '7|&3Rank&f:'
      - '8|Rank: %group%'
      - '10|&3World&f:'
      - 11|&b%world%
      - '13|&3Time&f:'
      - 14|&b%time%
      - '21|&3Teamspeak&f:'
      - 22|&bts.myserver.net
      - '23|&8&m                       '
      - '41|&3Store&f:'
      - 42|&bshop.myserver.net
      - '43|&8&m                       '
      groups:
        staff:
          slots:
          - 24-40
          display-condition: permission:tab.staff
        players:
          slots:
          - 44-80
ping-spoof:
  enabled: false
  value: 0
placeholders:
  date-format: dd.MM.yyyy
  time-format: '[HH:mm:ss / h:mm a]'
  time-offset: 0
  register-tab-expansion: false
placeholder-output-replacements:
  '%essentials_vanished%':
    'yes': '&7| Vanished'
    'no': ''
conditions:
  nick:
    conditions:
    - '%player%=%essentials_nickname%'
    true: '%player%'
    false: ~%essentials_nickname%
placeholder-refresh-intervals:
  default-refresh-interval: 500
  '%server_uptime%': 1000
  '%server_tps_1_colored%': 1000
  '%server_unique_joins%': 5000
  '%player_health%': 200
  '%player_ping%': 1000
  '%vault_prefix%': 1000
  '%rel_factionsuuid_relation_color%': 1000
assign-groups-by-permissions: false
primary-group-finding-list:
- Owner
- Admin
- Mod
- Helper
- default
permission-refresh-interval: 1000
debug: false
mysql:
  enabled: false
  host: 127.0.0.1
  port: 3306
  database: tab
  username: user
  password: password
  useSSL: true
proxy-support:
  enabled: true
  type: PLUGIN
  plugin:
    name: RedisBungee
  redis:
    url: redis://:password@localhost:6379/0
  rabbitmq:
    exchange: plugin
    url: amqp://guest:guest@localhost:5672/%2F
  channel-name-suffix: TAB
per-world-playerlist:
  enabled: false
  allow-bypass-permission: false
  ignore-effect-in-worlds:
  - ignoredworld
  - build
  shared-playerlist-world-groups:
    lobby:
    - lobby1
    - lobby2
    minigames:
    - paintball
    - bedwars
compensate-for-packetevents-bug: false
global-playerlist:
  enabled: false
  display-others-as-spectators: false
  display-vanished-players-as-spectators: true
  isolate-unlisted-servers: false
  update-latency: false
  spy-servers:
  - spyserver1
  - spyserver2
  server-groups:
    lobbies:
    - lobby1
    - lobby2
    group2:
    - server1
    - server2
use-bukkit-permissions-manager: false
use-online-uuid-in-tablist: true
config-version: 5
components:
  minimessage-support: true
  disable-shadow-for-heads: true
