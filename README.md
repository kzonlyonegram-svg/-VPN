# -VPN
российские приложения (банки, Госуслуги, маркетплейсы) шли напрямую, а всё остальное через VPN. Вот конфиг маршрутизации для Happ:
{
  "Name": "Мой RU роутинг",
  "GlobalProxy": "true",
  "UseChunkFiles": "true",
  "RemoteDns": "8.8.8.8",
  "DomesticDns": "77.88.8.8",
  "RemoteDNSType": "DoH",
  "RemoteDNSDomain": "https://8.8.8.8/dns-query",
  "RemoteDNSIP": "8.8.8.8",
  "DomesticDNSType": "DoH",
  "DomesticDNSDomain": "https://common.dot.dns.yandex.net/dns-query",
  "DomesticDNSIP": "77.88.8.8",
  "Geoipurl": "https://cdn.jsdelivr.net/gh/hydraponique/roscomvpn-geoip@latest/release/geoip.dat",
  "Geositeurl": "https://cdn.jsdelivr.net/gh/hydraponique/roscomvpn-geosite@latest/release/geosite.dat",
  "LastUpdated": "1778999351",
  "DnsHosts": {
    "lkfl2.nalog.ru": "213.24.64.175",
    "lknpd.nalog.ru": "213.24.64.181"
  },
  "RouteOrder": "block-proxy-direct",
  "DirectSites": [
    "domain:ru",
    "domain:su",
    "domain:xn--p1ai",
    "domain:sberbank.com",
    "domain:tbank.ru",
    "domain:tinkoff.ru",
    "domain:alfabank.ru",
    "domain:vtb.ru",
    "domain:gosuslugi.ru"
  ],
  "DirectIp": [
    "geoip:direct",
    "geoip:private"
  ],
  "ProxySites": [],
  "ProxyIp": [],
  "BlockSites": [],
  "BlockIp": [],
  "DomainStrategy": "IPIfNonMatch",
  "FakeDNS": "false"
}
