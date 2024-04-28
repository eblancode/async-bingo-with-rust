# Asynchronous Bingo

The game is designed for teams of 4 people each.

## Setup

1. Each team member is assigned an index from 1 to 4.
2. Each team member is randomly assigned one of four tasks (`task_a`, `task_b`, `task_c`, `task_d`).
3. Each team member gets a scratch paper for manual calculations.
4. Each team gets one shared pen.
5. Each team gets 8 small pieces of paper for passing results between tasks.

## Gameplay

### Team Rules

1. Each person can be in one of three states:
    - **waiting** for results from others or external input,
    - **calculating** results using the shared pen,
    - **finished** with their task.
2. Only one person can calculate at a time using the shared pen.
3. Results are passed between team members using the small pieces of paper.
4. If a team member reaches the instruction `println!("[B] BINGO: {result}")` with the correct result, the team wins.

### Turn-Taking

1. The game master continuously calls out indices from 1 to 4.
2. The team member with the called index can take action if they have all necessary data and the pen is available.

### External Data

1. Two tasks require data from an external source, which will be provided by the game master during the game.

# Variants

- Using 2 pens to represent two processors
- Introducing limited communication channels
- Using rendezvous channels for communication