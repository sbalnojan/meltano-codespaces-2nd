FROM meltano/meltano:v2.9.0-python3.10

WORKDIR /home/

COPY . .


# To query results.
RUN pip install duckdb

ENV PATH="$PATH:/venv/bin/meltano"

RUN cd ../home/ && ls
RUN ls
RUN meltano install loaders
RUN meltano install extractors
RUN meltano install mappers
