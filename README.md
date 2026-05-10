# CPU Monitor

A containerized monitoring solution for system metrics collection and visualization using Prometheus and Grafana.

## Architecture

The application follows a three-tier monitoring stack architecture:

- **Node Exporter**: Collects system metrics (CPU, memory, disk, network) from the host machine
- **Prometheus**: Time-series database that scrapes metrics from Node Exporter at 5-second intervals
- **Grafana**: Web-based visualization platform for creating dashboards and monitoring insights

All services communicate via Docker networking with Prometheus aggregating data from Node Exporter and Grafana querying Prometheus for visualization.

## Setup Steps

1. **Prerequisites**: Install Docker and Docker Compose

2. **Start the services**:
   ```bash
   docker-compose up -d
   ```

3. **Access the services**:
   - Prometheus: http://localhost:9090
   - Grafana: http://localhost:3000 (default credentials: admin/admin)
   - Node Exporter: http://localhost:9100

4. **Configure Grafana**:
   - Add Prometheus as a data source (URL: http://prometheus:9090)
   - Create dashboards to visualize metrics

## Dashboard Screenshots

### Prometheus Targets
Screenshot showing Node Exporter and Prometheus endpoints in Prometheus UI

### Grafana Dashboard
Example dashboard with CPU, memory, and disk usage metrics

## Tech Stack

- **Node Exporter**: Prometheus exporter for hardware and OS metrics
- **Prometheus**: Open-source time-series database and monitoring system
- **Grafana**: Open-source analytics and visualization platform
- **Docker**: Containerization platform
- **Docker Compose**: Multi-container orchestration
