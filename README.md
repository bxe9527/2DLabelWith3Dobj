# 2D标签跟随3D物体
  private Vector2 WorldToUIPoint(Vector3 worldGo)
    {
        Vector2 pos;
        RectTransformUtility.ScreenPointToLocalPointInRectangle(uiCanvas.GetComponent<RectTransform>(),
             Camera.main.().WorldToScreenPoint(worldGo), Camera.main, out pos);
        return pos;
    }
