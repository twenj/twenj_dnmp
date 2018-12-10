ARG ES_VERSION
FROM elasticsearch:${ES_VERSION}
ARG ES_IK_VERSION
ARG ES_PINYIN_VERSION

RUN /usr/share/elasticsearch/bin/elasticsearch-plugin install https://github.com/medcl/elasticsearch-analysis-pinyin/releases/download/v${ES_PINYIN_VERSION}/elasticsearch-analysis-pinyin-${ES_PINYIN_VERSION}.zip \
 && /usr/share/elasticsearch/bin/elasticsearch-plugin install https://github.com/medcl/elasticsearch-analysis-ik/releases/download/v${ES_IK_VERSION}/elasticsearch-analysis-ik-${ES_IK_VERSION}.zip
