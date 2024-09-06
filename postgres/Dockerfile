# Use the official PostgreSQL image from the Docker Hub
FROM postgres:latest

# Set environment variables for PostgreSQL
ENV POSTGRES_USER=pet_admin
ENV POSTGRES_PASSWORD=pet_admin
ENV POSTGRES_DB=pet_db

# Expose the PostgreSQL port
EXPOSE 5432

# Copy any initialization scripts 
COPY ./init-scripts/ /docker-entrypoint-initdb.d/

# Start the PostgreSQL server
CMD ["postgres"]