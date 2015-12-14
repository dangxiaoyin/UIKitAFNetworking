//
//  UITableView+Expanded.m
//  xxt_xj
//
//  Created by Yang on 14/12/3.
//  Copyright (c) 2014年 Points. All rights reserved.
//

#import "UITableView+Expanded.h"

@implementation UITableView (Expanded)
- (BOOL) scrolledToBottom
{
    return self.contentOffset.y >= (self.contentSize.height - self.bounds.size.height);
}

- (void)setScrolledToBottom:(BOOL)scrolledToBottom {
    NSInteger lastSection = [self.dataSource numberOfSectionsInTableView:self] - 1;
    NSInteger rowIndex = [self.dataSource tableView:self numberOfRowsInSection:lastSection] - 1;
    
    if(rowIndex >= 0) {
        NSIndexPath *indexPath = [NSIndexPath indexPathForRow:rowIndex inSection:lastSection];
        [self scrollToRowAtIndexPath:indexPath atScrollPosition:UITableViewScrollPositionBottom animated:scrolledToBottom];
    }

}
// Scrolls the UITableView to the bottom of the last row
//- (void)scrollToBottom:(BOOL)animated
//{
//    NSInteger lastSection = [self.dataSource numberOfSectionsInTableView:self] - 1;
//    NSInteger rowIndex = [self.dataSource tableView:self numberOfRowsInSection:lastSection] - 1;
//    
//    if(rowIndex >= 0) {
//        NSIndexPath *indexPath = [NSIndexPath indexPathForRow:rowIndex inSection:lastSection];
//        [self scrollToRowAtIndexPath:indexPath atScrollPosition:UITableViewScrollPositionBottom animated:animated];
//    }
//}

@end
