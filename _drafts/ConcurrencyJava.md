#Strategies to avoid synchronized (or locks) blocks (whe possible)

Synchronized blocks and Lock objects (introduced in Java 7?) are great tools for developers working in multi-threaded
environments.
However using these features always will have a performance penalty, because at some point, one or more threads will
have to wait for some other thread finishes doing whatever is doing with the shared resource.

The idea of this post is show some other features Java language has and sometimes can be used instead of synchronized
and Lock blocks to manage shared resources in a multi-threaded environments.

## Atomic's
- Atomic Boolean, Integer, Double, etc)
- Atomic Reference, AtomicMarkableReference and AtomicStampedReference

## Concurrent Collections
- Concurrent HashMap, etc
