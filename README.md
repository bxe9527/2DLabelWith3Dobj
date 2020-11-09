# 2D标签跟随3D物体
  private Camera _camera;//如果是MainCamera  
  private Vector2 WorldToUIPoint(Vector3 worldGo)
    {
        Vector2 pos;
        RectTransformUtility.ScreenPointToLocalPointInRectangle(uiCanvas.GetComponent<RectTransform>(),
             _camera.().WorldToScreenPoint(worldGo), Camera.main, out pos);//如果是MainCamera  Camera.main 参数为null
        return pos;
    }
