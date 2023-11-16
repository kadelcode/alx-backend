# Pagination
## Resources
 - [REST API Design: Pagination](https://www.moesif.com/blog/technical/api-design/REST-API-Design-Filtering-Sorting-and-Pagination/#pagination)
 - [HATEOAS](https://en.wikipedia.org/wiki/HATEOAS)

## Learning Objectives
- How to paginate a dataset with simple page and page_size parameters
- How to paginate a dataset with hypermedia metadata
- How to paginate in a deletion-resilient manner

## Setup: Popular_Baby_Names.csv
[use this data file](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/misc/2020/5/7d3576d97e7560ae85135cc214ffe2b3412c51d7.csv?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20231116%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20231116T194259Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=6a184a65381ef61455dddab4e14fd5e583620c18932810ded9f7b41f94a2e111) for your project

## Task
### 0. Simple helper function
Write a function named ```index_range``` that takes two integer arguments ```page``` and ```page_size```.

The function should return a tuple of size two containing a start index and an end index corresponding to the range of indexes to return in a list for those particular pagination parameters.

Page numbers are 1-indexed, i.e. the first page is page 1.
