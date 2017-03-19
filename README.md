# FlexibleHeaderView
FlexibleHeaderView is Qt widget extending QHeaderView with proportional column resizing.

For example, if you want to specify proportions for some columns:

```c++
FlexibleHeaderView *headerView = new FlexibleHeaderView(Qt::Horizontal);
headerView->setSectionProportion(1, 0.2);
headerView->setSectionProportion(2, 0.4);
headerView->setSectionProportion(4, 0.1);
```

Note, that it is not necessary to wath out for the sum of proportions, in each case they will be correctly normalized.

When user resizes columns, their proportions are being correctly updated.
