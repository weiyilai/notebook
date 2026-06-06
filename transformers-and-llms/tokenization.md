# Tokenization

Models understand numbers not text, we need to do something that makes the models to understand Natural language text&#x20;

Ex:  A Cute teddy bear is reading&#x20;

Unit of text is called token



**Arbitrary**: `A`, `cute`, `teddy bear`, `is`, `reading`, `.`&#x20;

**Word**:  `A`, `cute`, `teddy`, `bear` , `is`, `reading`, `.`&#x20;

**Sub word:** leveraging the roots of words,&#x20;

con -> make the sequence longer

&#x20;`A`, `cute`, `ted`,`##dy` ,`bear` , `is`, `read`,`##ing` ,`.`&#x20;



**Character level tokenizer:** each character is split into token



| Method          | Pros                                                                               | Cons                                                                            |
| --------------- | ---------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| Word Level      | <ul><li>Simple</li><li>Interpretable</li></ul>                                     | <ul><li>Risk of OOV</li><li>Does not leverage knowledge of root</li></ul>       |
| Sub word level  | <ul><li>Leverages common prefix and suffix</li><li>Learned from the data</li></ul> | <ul><li>Risk of OOV, though less than word-level</li></ul>                      |
| character level | <ul><li>Small change of OOV</li><li>RoBUsT tO CASinG anD misPeliNgS</li></ul>      | <ul><li>Makes computation slower</li><li>Embeddings not interpretable</li></ul> |





