#####################################################################################################    
new license: b4vZ+#m1hL4BmO?91mtr-Hbm  
  
How to update the license: replace the content of License.txt file which is in installation directory
with the new license.
##################################################################################################### 


# PCDViewer
It is a lightweight and powerful point cloud visualization software, which supports PCD, ply, Las etc., easily opens massive point cloud data, supports multi-mode and multi field rendering for point cloud and convenient query and measurement of points, which can be applied to surveying and mapping, high-precision map, SLAM and other fields.

一款轻量而功能强大的点云可视化软件，支持pcd, ply, las等多种格式，轻松打开海量点云数据，支持多方式多字段渲染点云，对点进行方便的查询和量测，可应用于测绘、高精地图、SLAM等领域。

# Release Page on CSDN  
https://blog.csdn.net/Jacky_546287052/article/details/118074205?spm=1001.2014.3001.5502

![image](https://github.com/XuShengpan/PCDViewer/blob/master/1.png)

## Shortcut key
P/p   Pan quickly/slowly      使平移速度变快/变慢  
R/r   Rotate quickly/slowly   使旋转速度变快/变慢  
Z/z   Zoom quickly/slowly     使缩放速度变快/变慢  
Shift + r   Start/Stop auto rotating    开启/停止 自动旋转  
  
S/s   Show points bigger/smaller  使点显示变大/变小  
Alt + X    snap a picture for current window  截图
  
H     Rotate horizontally only (i.e. disable rotate vertically)   仅允许水平旋转（即禁用竖直旋转）  
V     Rotate verticaly only (i.e. disable rotate horizontally)    仅允许竖直旋转（即禁用水平旋转）  

Alt + right_button_press on LayerTree space : create folder item. This can be used when there is no free space for creating new tree items.  
Layer Tree操作空间被占满时，可以在点击鼠标右键的同时按住Alt键，就可以弹出”Add Folder”菜单选项了。 
  
## Important Features
1. LAS 1.2 and any format that obey PCL PCD/PLY format files can be loaded and visualization;    
   LAS 1.2和任何满足PCL PCD/PLY 格式规范的点云文件都可以被加载和显示；  
2. You can render the point cloud as any field conveniently；  
   可以方便地按任意字段渲染点云；  
3. For a given field, multiple rendering styles are supported, including color table, random color and continuous color;    
   对指定的字段，提供了多种渲染方式，包括颜色表、随机色和连续色；  
5. Edit for color table is supported;  
   支持编辑颜色表；  
6. Query for point coordinate and measure for distance between two points are supported;  
   支持对点的坐标查询和点间距离的量测；  
7. Provides a MAGNIFIER tool to take a closer obsveration to a specific location, and tool can also used to selected a roaming center for the scene;  
   提供了一个放大镜工具对指定点观看，这个工具同时也可用来指定场景的漫游中心点;  
8. Filter by range is supported (can be found named "Beyond Strategy" in historgam window), you can show points only in a specific range, e.g. filter by elevation， filter by timestamps etc.  
   支持按范围过滤显示的点云(直方图控件中的"Beyond Strategy"选项)，比如可以按高程过滤、按时间戳过滤。
9. It is supported to show mapping result with a pose file. You can load the pose file before loading point cloud files.  
   Pose file format:  
   frame_id  timestamp  x   y   z  qx  qy  qz  qw  
   frame_id: the base_name of the pcd file (e.g 1.pcd, the base_name is 1)  
             it is suggested that the base_name name after the id or timestamp.  
   timestamp: time stamp of the point cloud  
   x, y, z : position  
   qx, qy, qz, qw: normalized quaternion  
   There is a demo pose file in test_data folder in the installation path.  
   
   支持按pose显示点云拼接效果。在加载单帧点云文件前，可以先加载pose文件以显示点云拼接效果。  
   Pose 文件的格式：  
   frame_id  timestamp  x   y   z  qx  qy  qz  qw  
   在安装目录的test_data文件夹下有一个样例文件。  
10. Filter ground and label for point cloud is supported, you can filter ground points by pop menu of the point cloud item in LayerTree, and use POLYGON SELECTION LABEL tool and Diffuse LABEL TOOL to label the point cloud. After labeling, the point cloud item will add a star (*) tag at the front of its name to identify the label state, the user can export label result with Save Label PCD button in pop menu of the point cloud item.    
    软件提供了点云滤波和编辑功能。点云地面滤波是点云处理中常用功能，软件提供了一个点云地面滤波器，对城区和山区、车载和机载等点云都能取得不错的地面滤波效果，点云滤波中的参数可以在Ground Filter Parameters Config中设置。软件提供了“多边形选点(Polygon Label Tool)”和“扩散选点(Diffuse Label Tool)”标注工具，对带label或classification字段的点云数据，通过标注工具选中点，即可将点分至目标类别，目标类别通过组合框指定。Layer Tree中的文件名前面会带星号以标识状态。用户可以通过弹出菜单中的Save Label PCD 按钮保存滤波和编辑结果。
 
