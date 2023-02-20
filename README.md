# Dragonfly

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
  
