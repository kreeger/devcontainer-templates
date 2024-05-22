ARG SWIFT_VERSION="5.10"
FROM swift:${SWIFT_VERSION}

ARG SWIFT_FORMAT_VERSION="510.1.0"
RUN git clone --depth 1 --branch $SWIFT_FORMAT_VERSION https://github.com/apple/swift-format.git &&\
    cd swift-format &&\
    swift build -c release &&\
    mkdir -p /usr/local/bin &&\
    mv .build/release/swift-format /usr/local/bin/swift-format
