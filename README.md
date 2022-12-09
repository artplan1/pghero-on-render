# PGhero on Render.com

Pghero performance dashboard for Postgres on Render

This is an example repo with a Dockerfile for running Pghero as a web service on Render.

You can use it to easily check performance of your PostgreSQL instances running on Render.


## Deployment

1. Create a [new Web Service on Render](https://dashboard.render.com/web/new), and enter [link to this repo](https://github.com/artplan1/pghero-on-render) in Public Git repository field.
1. Make sure the Environment is set to Docker, and enter a name for the service.
1. Open advanced settings and set following environment variables:
  
  - `DATABASE_URL` - private connection string to your pg instance
  - `PGHERO_USERNAME` - username to open pghero interface
  - `PGHERO_PASSWORD` - password to open pghero interface

Click Save and you’re good to go! Once ready, your Pghero instance will be available on your render.com URL.

---

More Pghero documentation: https://github.com/ankane/pghero/blob/master/guides/Docker.md
