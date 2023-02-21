# Dragonfly
  По информации из [источника](https://medium.com/geekculture/dragonfly-a-high-performance-in-memory-data-store-for-distributed-systems-248edc02b0c6#:~:text=Dragonfly%20is%20an%20open%2Dsource%20distributed%20data%20storage%20system%20designed%20to%20provide%20a%20high%2Dperformance%20and%20highly%20available%20in%2Dmemory%20storage%20option.%20It%20is%20built%20to%20handle%20large%20amounts%20of%20data%20and%20handle%20high%20read%20and%20write%20loads%2C%20with%20a%20focus%20on%20low%2Dlatency%20data%20access.):
  >Dragonfly is an open-source distributed data storage system designed to provide a high-performance and __highly__ __available__ in-memory storage option. It is built to handle large amounts of data and handle high read and write loads, with a focus on __low-latency__ data access.
  
  Т.е. Dragonfly относится к CA
# ScyllaDB
  Основываясь на [источнике](https://docs.scylladb.com/stable/architecture/architecture-fault-tolerance.html#:~:text=Scylla%20chooses%20availability,be%20highly%20available.):
  > Scylla chooses availability and partition tolerance over consistency, such that:
  > - t’s impossible to be both consistent and highly available during a network partition;
  > - If we sacrifice consistency, we can be highly available.
  
  можно сделать вывод, что ScyllaDB относится к AP

# ArenadataDB
  Согласно [источнику](https://arenadata.tech/products/arenadata-db/), ArenadataDB соответсвует __Partition__ __Tolerance__ и
  
  имеет полное соответствие принципам строгой 
  изоляции транзакции (принципы ACID), т.е. выполняется __Consistency__.
  
  Но из-за ACID теряется Availability.
  
  Значит, ArenadataDB относится к CP
  
