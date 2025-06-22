# Collision Handling

Objective: Handle hash collisions using chained nodes.

Tasks:
1. Traverse existing chains to find insertion/update points
2. Implement proper synchronization for chain modifications
3. Use the first node's lock to protect the entire bin

Key Concepts: When bins are not empty, updates require locks, using the first node of a bin list as the lock for the entire bin lib.rs:112-120.