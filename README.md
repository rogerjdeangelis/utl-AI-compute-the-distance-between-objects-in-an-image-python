# utl-AI-compute-the-distance-between-objects-in-an-image-python
AI compute the distance between objects in an image python 
    AI compute the distance between objects in an image python                                                                              
                                                                                                                                            
    Python graphic output                                                                                                                   
    https://tinyurl.com/ya5n5ehm                                                                                                            
    https://github.com/rogerjdeangelis/utl-AI-compute-the-distance-between-objects-in-an-image-python/blob/master/lower.png                 
                                                                                                                                            
    https://tinyurl.com/yb6v54qd                                                                                                            
    https://github.com/rogerjdeangelis/utl-AI-compute-the-distance-between-objects-in-an-image-python/blob/master/upper.png                 
                                                                                                                                            
    https://tinyurl.com/y7pkacxm                                                                                                            
    https://github.com/rogerjdeangelis/utl-AI-compute-the-distance-between-objects-in-an-image-python                                       
                                                                                                                                            
    Also see digitizer repo                                                                                                                 
    github                                                                                                                                  
    https://github.com/rogerjdeangelis?tab=repositories&q=digitize&type=&language=                                                          
                                                                                                                                            
    This is the source for this post and provides excellent documentation.                                                                  
    https://tinyurl.com/ydd9vkkm                                                                                                            
    https://www.pyimagesearch.com/2016/04/04/measuring-distance-between-objects-in-an-image-with-opencv/                                    
                                                                                                                                            
    INSTALLIN CV2 IS A LITTLE TRICKY                                                                                                        
                                                                                                                                            
    I downloaded and unzipped the download and copied                                                                                       
    https://opencv-python-tutroals.readthedocs.io/en/latest/py_tutorials/py_setup/py_setup_in_windows/py_setup_in_windows.html              
    copy                                                                                                                                    
    cv2.cp38-win_amd64.pyd                                                                                                                  
    to                                                                                                                                      
    C:\python38\Lib\site-packages                                                                                                           
                                                                                                                                            
    /*                   _                                                                                                                  
    (_)_ __  _ __  _   _| |_                                                                                                                
    | | `_ \| `_ \| | | | __|                                                                                                               
    | | | | | |_) | |_| | |_                                                                                                                
    |_|_| |_| .__/ \__,_|\__|                                                                                                               
            |_|                                                                                                                             
    */                                                                                                                                      
                                                                                                                                            
    https://tinyurl.com/ydevuu64                                                                                                            
    https://github.com/rogerjdeangelis/utl-AI-compute-the-distance-between-objects-in-an-image-python/blob/master/displt.png                
                                                                                                                                            
    %let image=d:\png\displt.png;                                                                                                           
    %let width=0.955; ** the radius of the leftmost project                                                                                 
                                                                                                                                            
    * CREATE IMAGE;                                                                                                                         
                                                                                                                                            
    %utlfkil(d:\png\displt.png);                                                                                                            
                                                                                                                                            
    data have;                                                                                                                              
      x=5;y=5;sex="F";size=10;output;                                                                                                       
      x=8;y=2;sex="M";size=20;output;                                                                                                       
      x=8;y=8;sex="U";size=30;output;                                                                                                       
    run;quit;                                                                                                                               
                                                                                                                                            
    ods listing gpath="d:\png" style=analysis;                                                                                              
    ods graphics on / reset=index width=5in height=5in imagefmt=png imagename='displt' noborder;                                            
    proc sgplot data=have NOAUTOLEGEND NOBORDER;                                                                                            
    title;                                                                                                                                  
    styleattrs datasymbols=(circlefilled squarefilled starfilled);                                                                          
    scatter x=X y=Y  / group=sex markerattrs=(size=75px) ;                                                                                  
    xaxis DISPLAY=NONE ;                                                                                                                    
    yaxis DISPLAY=NONE ;                                                                                                                    
    run;                                                                                                                                    
    ods graphics off;                                                                                                                       
    ods listing;                                                                                                                            
                                                                                                                                            
                                                                                                                                            
                                                                                                                                            
     +--------------------------+                                                                                                           
     |                ___       |                                                                                                           
     |               /   \      |                                                                                                           
     |              |     |     |                                                                                                           
     |               \___/      |                                                                                                           
     |                          |                                                                                                           
     |                          |                                                                                                           
     |                          |                                                                                                           
     |     ___                  |                                                                                                           
     |    /   \  Reference      |                                                                                                           
     |   | @ @ | quarter 0.995in|                                                                                                           
     |   |  ^  | wide           |                                                                                                           
     |    \___/                 |                                                                                                           
     |   [.995in]               |                                                                                                           
     |               _____      |                                                                                                           
     |              |     |     |                                                                                                           
     |              |     |     |                                                                                                           
     |              |_____|     |                                                                                                           
     |                          |                                                                                                           
     +--------------------------+                                                                                                           
                                                                                                                                            
    /*           _               _                                                                                                          
      ___  _   _| |_ _ __  _   _| |_                                                                                                        
     / _ \| | | | __| `_ \| | | | __|                                                                                                       
    | (_) | |_| | |_| |_) | |_| | |_                                                                                                        
     \___/ \__,_|\__| .__/ \__,_|\__|                                                                                                       
                    |_|                                                                                                                     
    */                                                                                                                                      
                                                                                                                                            
     +--------------------------+                                                                                                           
     |                ___       |                                                                                                           
     |               /   \      |                                                                                                           
     |              |     |     |                                                                                                           
     |              /\___/      |                                                                                                           
     |             /            |                                                                                                           
     |            /             |                                                                                                           
     |           / 4.3in        |                                                                                                           
     |     ___  /               |                                                                                                           
     |    /   \/                |                                                                                                           
     |   | @ @ |                |                                                                                                           
     |   |  ^  |                |                                                                                                           
     |    \___/ \ 4.3in         |                                                                                                           
     |           \              |                                                                                                           
     |            \  _____      |                                                                                                           
     |             \|     |     |                                                                                                           
     |              |     |     |                                                                                                           
     |              |_____|     |                                                                                                           
     |                          |                                                                                                           
     +--------------------------+                                                                                                           
                                                                                                                                            
    From Python                                                                                                                             
                                                                                                                                            
    d:/txt/file.txt                                                                                                                         
                                                                                                                                            
    4.283279858874036                                                                                                                       
    4.382173237986379                                                                                                                       
    4.348556627546038 ** midpoint to midpoint upper                                                                                         
    4.248880894648565                                                                                                                       
    4.3155202533672385                                                                                                                      
                                                                                                                                            
    4.281986533821403                                                                                                                       
    4.281986533821403                                                                                                                       
    4.281986533821403 ** midpoint to midpoint lower                                                                                         
    4.281986533821403                                                                                                                       
    4.281986533821403                                                                                                                       
                                                                                                                                            
    WORK.WANT total obs=2                                                                                                                   
                                                                                                                                            
                     OBJECT                    DISTANCE                                                                                     
                                                                                                                                            
      leftmost object to upper right object     4.34856                                                                                     
      leftmost object to lower right object     4.28199                                                                                     
                                                                                                                                            
    /*                                                                                                                                      
     _ __  _ __ ___   ___ ___  ___ ___                                                                                                      
    | `_ \| `__/ _ \ / __/ _ \/ __/ __|                                                                                                     
    | |_) | | | (_) | (_|  __/\__ \__ \                                                                                                     
    | .__/|_|  \___/ \___\___||___/___/                                                                                                     
    |_|                                                                                                                                     
    */                                                                                                                                      
                                                                                                                                            
                                                                                                                                            
    %let image=d:\png\displt.png;                                                                                                           
    %let width=0.955; ** the radius of the leftmost project;                                                                                
                                                                                                                                            
    * best;                                                                                                                                 
    %utl_submit_py64_38(resolve('                                                                                                           
    from scipy.spatial import distance as dist;                                                                                             
    from imutils import perspective;                                                                                                        
    from imutils import contours;                                                                                                           
    import numpy as np;                                                                                                                     
    import pandas as pd;                                                                                                                    
    import argparse;                                                                                                                        
    import imutils;                                                                                                                         
    import cv2;                                                                                                                             
    def midpoint(ptA, ptB):;                                                                                                                
    .     return ((ptA[0] + ptB[0]) * 0.5, (ptA[1] + ptB[1]) * 0.5);                                                                        
    /* construct the argument parse and parse the arguments                                                                                 
    ap = argparse.ArgumentParser();                                                                                                         
    ap.add_argument("-i", "--image", required=True,;                                                                                        
    .      help="path to the input image");                                                                                                 
    ap.add_argument("-w", "--width", type=float, required=True,;                                                                            
    .     help="width of the left-most object in the image (in inches)");                                                                   
    args = vars(ap.parse_args());                                                                                                           
    */                                                                                                                                      
    image="&image";                                                                                                                         
    width=&width;                                                                                                                           
    /* load the image, convert it to grayscale, and blur it slightly */                                                                     
    image = cv2.imread(image);                                                                                                              
    gray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY);                                                                                         
    gray = cv2.GaussianBlur(gray, (7, 7), 0);                                                                                               
    /* perform edge detection, then perform a dilation + erosion to */                                                                      
    /* close gaps in between object edges */                                                                                                
    edged = cv2.Canny(gray, 50, 100);                                                                                                       
    edged = cv2.dilate(edged, None, iterations=1);                                                                                          
    edged = cv2.erode(edged, None, iterations=1);                                                                                           
    /* find contours in the edge map */                                                                                                     
    cnts = cv2.findContours(edged.copy(), cv2.RETR_EXTERNAL,;                                                                               
          cv2.CHAIN_APPROX_SIMPLE);                                                                                                         
    cnts = imutils.grab_contours(cnts);                                                                                                     
    /* sort the contours from left-to-right and, then initialize the */                                                                     
    /* distance colors and reference object */                                                                                              
    (cnts, _) = contours.sort_contours(cnts);                                                                                               
    colors = ((0, 0, 255), (240, 0, 159), (0, 165, 255), (255, 255, 0),                                                                     
          (255, 0, 255));                                                                                                                   
    refObj = None;                                                                                                                          
    df=pd.DataFrame(0, index=[1], columns=["DIS"]);                                                                                         
    /* loop over the contours individually */                                                                                               
    for c in cnts:;                                                                                                                         
          /* if the contour is not sufficiently large, ignore it */                                                                         
    .     if cv2.contourArea(c) < 100:;                                                                                                     
    .           continue;                                                                                                                   
          /* compute the rotated bounding box of the contour */                                                                             
    .     box = cv2.minAreaRect(c);                                                                                                         
    .     box = cv2.cv.BoxPoints(box) if imutils.is_cv2() else cv2.boxPoints(box);                                                          
    .     box = np.array(box, dtype="int");                                                                                                 
          /* order the points in the contour such that they appear */                                                                       
          /* in top-left, top-right, bottom-right, and bottom-left */                                                                       
          /* order, then draw the outline of the rotated bounding  */                                                                       
          /* box */                                                                                                                         
    .     box = perspective.order_points(box);                                                                                              
          /* compute the center of the bounding box */                                                                                      
    .     cX = np.average(box[:, 0]);                                                                                                       
    .     cY = np.average(box[:, 1]);                                                                                                       
          /* if this is the first contour we are examining (i.e., */                                                                        
          /* the left-most contour), we presume this is the       */                                                                        
          /* reference object                                     */                                                                        
    .     if refObj is None:;                                                                                                               
                /* unpack the ordered bounding box, then compute the   */                                                                   
                /* midpoint between the top-left and top-right points, */                                                                   
                /* followed by the midpoint between the top-right and  */                                                                   
                /* bottom-right                                        */                                                                   
    .           (tl, tr, br, bl) = box;                                                                                                     
    .           (tlblX, tlblY) = midpoint(tl, bl);                                                                                          
    .           (trbrX, trbrY) = midpoint(tr, br);                                                                                          
                /* compute the Euclidean distance between the midpoints, */                                                                 
                /* then construct the reference object                   */                                                                 
    .           D = dist.euclidean((tlblX, tlblY), (trbrX, trbrY));                                                                         
    .           refObj = (box, (cX, cY), D / width);                                                                                        
    .           continue;                                                                                                                   
          /* draw the contours on the image */                                                                                              
    .     orig = image.copy();                                                                                                              
    .     cv2.drawContours(orig, [box.astype("int")], -1, (0, 255, 0), 2);                                                                  
    .     cv2.drawContours(orig, [refObj[0].astype("int")], -1, (0, 255, 0), 2);                                                            
          /* stack the reference coordinates and the object coordinates */                                                                  
          /* to include the object center                               */                                                                  
    .     refCoords = np.vstack([refObj[0], refObj[1]]);                                                                                    
    .     objCoords = np.vstack([box, (cX, cY)]);                                                                                           
          /* loop over the original points */                                                                                               
    .     for ((xA, yA), (xB, yB), color) in zip(refCoords, objCoords, colors):;                                                            
                /* draw circles corresponding to the current points and                                                                     
                /* connect them with a line */                                                                                              
    .           cv2.circle(orig, (int(xA), int(yA)), 5, color, -1);                                                                         
    .           cv2.circle(orig, (int(xB), int(yB)), 5, color, -1);                                                                         
    .           cv2.line(orig, (int(xA), int(yA)), (int(xB), int(yB)),;                                                                     
    .                 color, 2);                                                                                                            
                /* compute the Euclidean distance between the coordinates, */                                                               
                /* and then convert the distance in pixels to distance in  */                                                               
                /* units  */                                                                                                                
    .           D = dist.euclidean((xA, yA), (xB, yB)) / refObj[2];                                                                         
    .           (mX, mY) = midpoint((xA, yA), (xB, yB));                                                                                    
    .           cv2.putText(orig, "{:.1f}in".format(D), (int(mX), int(mY - 10)),;                                                           
    .                 cv2.FONT_HERSHEY_SIMPLEX, 0.55, color, 2);                                                                            
    .           with open("d:/txt/file.txt", "a") as f:;                                                                                    
    .                print(D, file=f);                                                                                                      
                /* show the output image */                                                                                                 
    .           cv2.imshow("Image", orig);                                                                                                  
    .           cv2.waitKey(0);                                                                                                             
    '));                                                                                                                                    
                                                                                                                                            
                                                                                                                                            
    /*                                                                                                                                      
    d:/txt/file.txt                                                                                                                         
                                                                                                                                            
    4.283279858874036                                                                                                                       
    4.382173237986379                                                                                                                       
    4.348556627546038                                                                                                                       
    4.248880894648565                                                                                                                       
    4.3155202533672385                                                                                                                      
    4.281986533821403                                                                                                                       
    4.281986533821403                                                                                                                       
    4.281986533821403                                                                                                                       
    4.281986533821403                                                                                                                       
    4.281986533821403                                                                                                                       
    */                                                                                                                                      
                                                                                                                                            
    data want;                                                                                                                              
      retain object;                                                                                                                        
      infile "d:/txt/file.txt";                                                                                                             
      input distance;                                                                                                                       
      select (_n_);                                                                                                                         
         when (3) do;                                                                                                                       
           object="leftmost object to upper right object";                                                                                  
           output;                                                                                                                          
         end;                                                                                                                               
         when (8) do;                                                                                                                       
           object="leftmost object to lower right object";                                                                                  
           output;                                                                                                                          
         end;                                                                                                                               
         otherwise;                                                                                                                         
      end;                                                                                                                                  
    run;quit;                                                                                                                               
                                                                                                                                            
    /*                                                                                                                                      
    Up to 40 obs WORK.WANT total obs=2                                                                                                      
                                                                                                                                            
    Obs                   OBJECT                    DISTANCE                                                                                
                                                                                                                                            
     1     leftmost object to upper right object     4.34856                                                                                
     2     leftmost object to lower right object     4.28199                                                                                
    */                                                                                                                                      
                                                                                                                                            
                                                                                                                                            
                                                                                                                                            
                                                                                                                                            
