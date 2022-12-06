FROM meltano/meltano:v2.9.0-python3.10

WORKDIR /home/

COPY . .


# To query results.
RUN pip install duckdb

#RUN meltano install extractors
#RUN meltano install loaders
#RUN meltano install mappers
ENV PATH="$PATH:/venv/bin/meltano"
