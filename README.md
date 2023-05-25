# Minecraft Cloudflared
Main purpose of this project is to expose dockerized Minecraft server without opening any ports on the local network with the help of Cloudflare Tunnel.
### Prerequisites

[Docker](https://docs.docker.com/get-docker/) / [Docker Compose](https://github.com/docker/compose#where-to-get-docker-compose)
[Cloudflare account / Domain which uses Cloudflare nameservers](https://developers.cloudflare.com/dns/zone-setups/full-setup/setup/)

### Quick Start

1. Get the tunnel token from the Zero Trust page
2. Clone the repo
   ```sh
   git clone https://github.com/takoine/minecraft-cloudflared.git
   ```
3. Enter your tunnel token in `docker-compose.yml`
   ```sh
   TUNNEL_TOKEN="{{token}}";
   ```
   Or export it as a environment variable
   ```sh
   export TUNNEL_TOKEN="{{token}}"
   ```
4. Run docker-compose
   ```sh
   docker-compose up -d
   ```



<!-- USAGE EXAMPLES -->
## Advanced Usage
For advanced usage consult the documentation of [Cloudflare Zero Trust](https://developers.cloudflare.com/cloudflare-one/connections/connect-apps/) and [itzg/minecraft-server repository](https://github.com/itzg/docker-minecraft-server)



<!-- ROADMAP -->
## Roadmap

- [ ] Terraform module



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. 

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



<!-- LICENSE -->
## License

Distributed under the GNUv3 License. See `LICENSE` for more information.
