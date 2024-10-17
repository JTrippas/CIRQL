# CIRQL: Conversational Information Retrieval Query Log

[CIRQL][jt] is created from a crowdsourcing experiment where workers could opt-in to
share the logs of their Google smart assistant devices. The entirety of this
data consists of over 600,000 interactions (either inputs from the users or
responses from the assistant) from 173 unique users. CIRQL is a strict subset
of the *user* interactions generated by a filtering process; the filtering
aimed to remove common commands and non-query interactions (like *turn off
the lights*) as well as any non-English inputs, addresses, phone numbers,
emojis, and so on.

The whole filtering process is described in the paper below.

## Dataset

The resulting dataset, CIRQL, contains 2,807 queries from 1,799 user sessions.
Session data is synthetic and derived using an inactivity period of 15 minutes.
The order of queries within a session is ascending chronological.
Therefore the first query of a session is time step `t1`, the second query is time step `t2`,
and so on.

[jt]: https://www.johannetrippas.com/papers/trippas2024re-evaluating.pdf

## Usage

If using the CIRQL dataset, please cite the paper:

```
@inproceedings{trippas2024reevaluating,
 author = {Trippas, Johanne R and Gallagher, Luke and Mackenzie, Joel},
 booktitle = {Proceedings of the 33rd ACM International Conference on Information and Knowledge Management},
 series = {CIKM '24},
 title = {Re-evaluating the Command-and-Control Paradigm in Conversational Search Interactions},
 year = {2024},
 doi = {doi.org/10.1145/3627673.3679588},
 address = {New York, NY, USA},
 location = {Boise, ID, USA},
 publisher = {ACM}
}
```
