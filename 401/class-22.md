# RecyclerView

RecyclerView is a view and it's the ViewGroup that contains the views containing data. It makes it easy to dispaly large sets of data.

As it's name says, RecyclerView recycles view such that when an item scrolls off screen, RecyclerView doesn't destroy its view but reuses it for new items that have scrolled onscreen. By this way improves peformance.

To build a RecyclerView, we need to use several classes that work together to build our list:

- `RecyclerView` class.

- View holder object for each element in the list, by extending `RecyclerView.ViewHolder`.

- To bind data to views, define adapter by extending `RecyclerView.Adapter`.

- To arrange elements in list we use layout manager in  `LayoutManager`  class.

The process of associating view to their data using an adapter is called _binding_.

