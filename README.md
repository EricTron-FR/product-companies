# ProductCompanies.eu

<div align="center">

![Website](https://img.shields.io/website?url=https%3A%2F%2Fproductcompanies.eu&up_message=online&up_color=0046FF&down_message=offline&down_color=FF9013&style=for-the-badge)
![React](https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react&logoColor=white)
![Fastify](https://img.shields.io/badge/Fastify-4-000000?style=for-the-badge&logo=fastify&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-6-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Leaflet](https://img.shields.io/badge/Leaflet-1.9-199900?style=for-the-badge&logo=leaflet&logoColor=white)

![Contributions](https://img.shields.io/badge/contributions-welcome-0046FF?style=for-the-badge)
![Made with Love](https://img.shields.io/badge/Made%20with-❤️-FF9013?style=for-the-badge)

</div>

---

> Discover Europe's best tech product companies building real products

**ProductCompanies.eu** is a curated directory showcasing European tech companies that build genuine, internally developed products. Explore opportunities through an interactive map, advanced filters, and detailed company information.

**🌐 Live Site:** [https://productcompanies.eu](https://productcompanies.eu)

![ProductCompanies.eu Screenshot](frontend/public/og-image.png)

## Overview

ProductCompanies.eu helps professionals discover real product-driven tech companies in Europe. Each entry highlights company details, tech stack, and hiring information, enabling users to explore authentic engineering opportunities.

## Features

- Interactive map with geographic company markers  
- Search by name, city, or country  
- Advanced filters by sector, tech stack, and remote options  
- Deep linking for sharing filtered results  
- Responsive design optimized for all devices  
- Keyboard shortcuts for quick navigation  
- Modern, lightweight UI built with performance in mind  

## Tech Stack

**Frontend**
- React — user interface  
- Leaflet — interactive maps  

**Backend**
- Fastify — high-performance Node.js framework  
- MongoDB — NoSQL database  
- Mongoose — schema modeling  

**Deployment**
- Nginx — reverse proxy  
- PM2 — process management  
- Let’s Encrypt — SSL certificates  
- Kimsufi — dedicated hosting  

## Database Schema

Each company entry follows this structure:

```javascript
{
  name: String,
  description: String,
  website: String,
  careers: String,
  logoUrl: String,
  location: {
    city: String,
    country: String,
    coordinates: [Number, Number]
  },
  sector: [String],
  techStack: [String],
  remote: Boolean,
  createdAt: Date,
  updatedAt: Date
}
``` 

## Contributing

We welcome suggestions from the community! You can help by:
- Suggesting companies that meet our criteria
- Reporting bugs or proposing feature ideas

### How to Suggest a Company

To be listed, a company must:
- Be a **product company** 
- Be **based in Europe**
- Be **actively developing tech products**
- Have a **public website and careers page**
- Employ engineers working on internal products

**To suggest a company**, open an [issue](../../issues/new) using the [company suggestion template](.github/COMPANY_SUGGESTION.md). All suggestions are manually reviewed and added by the maintainer.

## API Overview

### Companies
- `GET /api/companies` — Retrieve companies  
  - Optional filters: `?country=France&sector=Fintech&tech=React&remote=true`  
- `GET /api/companies/:id` — Retrieve a company by ID  

## Roadmap

Planned features for future versions include:
- Random company discovery  
- Dark mode  
- Sorting and ranking options  
- “We’re hiring” badges  
- Newsletter subscription  
- CSV export for filtered results  
- PWA support  
- Company metadata (size, founding year)  
- Popularity metrics and favorites  

## Acknowledgments

- Company logos provided by [Clearbit](https://clearbit.com)  
- Map tiles by [OpenStreetMap](https://www.openstreetmap.org)  
- Design inspiration from modern UI trends  

## Contact

Questions or suggestions?
- Open an [issue](../../issues)
- Visit [productcompanies.eu](https://productcompanies.eu)

---

Made with passion ❤️ for the European tech community.
