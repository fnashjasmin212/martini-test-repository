FROM lontiplatform/martini-server-runtime:2.6.0

ARG MR_LICENSE

WORKDIR /data

COPY [ "packages/new-package", "packages/new-package" ]
COPY /conf/overrides/override.properties conf/overrides/

ENV MR_PROPERTY_1=value
ENV MR_LICENSE=$MR_LICENSE

EXPOSE 9090

ENTRYPOINT ["sh", "/data/bin/toro-martini"]