ARG HADOOP_TAG
FROM infotechsoft/hadoop:${HADOOP_TAG}

ENV HDFS_CONF_dfs_namenode_name_dir=file:///hadoop/dfs/name
RUN mkdir -p /hadoop/dfs/name/checkpoint

ADD run.sh /run.sh
RUN chmod a+x /run.sh

CMD ["/run.sh"]
