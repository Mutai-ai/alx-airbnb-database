<mxfile host="app.diagrams.net" agent="Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/136.0.0.0 Safari/537.36" version="27.0.3">
  <diagram name="Page-1" id="rFuNGGrTgy3959ek8qQO">
    <mxGraphModel dx="872" dy="473" grid="1" gridSize="10" guides="1" tooltips="1" connect="1" arrows="1" fold="1" page="1" pageScale="1" pageWidth="850" pageHeight="1100" math="0" shadow="0">
      <root>
        <mxCell id="0" />
        <mxCell id="1" parent="0" />
        <mxCell id="N7N4YLxj38OcdQxVAtvY-1" value="User" style="swimlane;childLayout=stackLayout;horizontal=1;startSize=50;horizontalStack=0;rounded=1;fontSize=14;fontStyle=0;strokeWidth=2;resizeParent=0;resizeLast=1;shadow=0;dashed=0;align=center;arcSize=4;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="100" y="300" width="170" height="190" as="geometry">
            <mxRectangle x="110" y="300" width="70" height="50" as="alternateBounds" />
          </mxGeometry>
        </mxCell>
        <mxCell id="N7N4YLxj38OcdQxVAtvY-2" value="+user_id&amp;nbsp; &amp;nbsp; &amp;nbsp; &amp;nbsp; +password_hash&lt;div&gt;+first_name&lt;/div&gt;&lt;div&gt;+last_name&lt;/div&gt;&lt;div&gt;+email (UNIQUE, INDEXED)&lt;/div&gt;&lt;div&gt;+phone_number&lt;/div&gt;&lt;div&gt;+role&lt;/div&gt;&lt;div&gt;+created_at&lt;/div&gt;" style="align=left;strokeColor=none;fillColor=none;spacingLeft=4;spacingRight=4;fontSize=12;verticalAlign=top;resizable=0;rotatable=0;part=1;html=1;whiteSpace=wrap;" vertex="1" parent="N7N4YLxj38OcdQxVAtvY-1">
          <mxGeometry y="50" width="170" height="140" as="geometry" />
        </mxCell>
        <mxCell id="N7N4YLxj38OcdQxVAtvY-3" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;exitX=0.75;exitY=1;exitDx=0;exitDy=0;entryX=0.75;entryY=1;entryDx=0;entryDy=0;" edge="1" parent="N7N4YLxj38OcdQxVAtvY-1" source="N7N4YLxj38OcdQxVAtvY-1" target="N7N4YLxj38OcdQxVAtvY-2">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="N7N4YLxj38OcdQxVAtvY-4" value="Property" style="swimlane;childLayout=stackLayout;horizontal=1;startSize=50;horizontalStack=0;rounded=1;fontSize=14;fontStyle=0;strokeWidth=2;resizeParent=0;resizeLast=1;shadow=0;dashed=0;align=center;arcSize=4;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="360" y="300" width="160" height="190" as="geometry" />
        </mxCell>
        <mxCell id="N7N4YLxj38OcdQxVAtvY-5" value="+property_id&lt;div&gt;+host_id(FK&lt;/div&gt;&lt;div&gt;+name&lt;/div&gt;&lt;div&gt;+description&lt;/div&gt;&lt;div&gt;+location&lt;/div&gt;&lt;div&gt;+pricepernight&lt;/div&gt;&lt;div&gt;+created_at&lt;/div&gt;&lt;div&gt;+updated_at&lt;/div&gt;" style="align=left;strokeColor=none;fillColor=none;spacingLeft=4;spacingRight=4;fontSize=12;verticalAlign=top;resizable=0;rotatable=0;part=1;html=1;whiteSpace=wrap;" vertex="1" parent="N7N4YLxj38OcdQxVAtvY-4">
          <mxGeometry y="50" width="160" height="140" as="geometry" />
        </mxCell>
        <mxCell id="N7N4YLxj38OcdQxVAtvY-6" value="Booking" style="swimlane;childLayout=stackLayout;horizontal=1;startSize=50;horizontalStack=0;rounded=1;fontSize=14;fontStyle=0;strokeWidth=2;resizeParent=0;resizeLast=1;shadow=0;dashed=0;align=center;arcSize=4;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="630" y="300" width="160" height="190" as="geometry" />
        </mxCell>
        <mxCell id="N7N4YLxj38OcdQxVAtvY-7" value="+booking_id&lt;div&gt;+property_id(FK&lt;/div&gt;&lt;div&gt;+user_id(FK&lt;/div&gt;&lt;div&gt;+start_date&lt;/div&gt;&lt;div&gt;+end_date&lt;/div&gt;&lt;div&gt;+total_price&lt;/div&gt;&lt;div&gt;+status(pending, confirmend, cancelled)&lt;/div&gt;&lt;div&gt;+created_at&lt;/div&gt;" style="align=left;strokeColor=none;fillColor=none;spacingLeft=4;spacingRight=4;fontSize=12;verticalAlign=top;resizable=0;rotatable=0;part=1;html=1;whiteSpace=wrap;" vertex="1" parent="N7N4YLxj38OcdQxVAtvY-6">
          <mxGeometry y="50" width="160" height="140" as="geometry" />
        </mxCell>
        <mxCell id="N7N4YLxj38OcdQxVAtvY-11" value="Payment" style="swimlane;childLayout=stackLayout;horizontal=1;startSize=50;horizontalStack=0;rounded=1;fontSize=14;fontStyle=0;strokeWidth=2;resizeParent=0;resizeLast=1;shadow=0;dashed=0;align=center;arcSize=4;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="90" y="570" width="170" height="190" as="geometry" />
        </mxCell>
        <mxCell id="N7N4YLxj38OcdQxVAtvY-12" value="+payment_id&lt;div&gt;+booking_id(FK&lt;/div&gt;&lt;div&gt;+amount&lt;/div&gt;&lt;div&gt;+payment_date&lt;/div&gt;&lt;div&gt;+payment_method&lt;/div&gt;" style="align=left;strokeColor=none;fillColor=none;spacingLeft=4;spacingRight=4;fontSize=12;verticalAlign=top;resizable=0;rotatable=0;part=1;html=1;whiteSpace=wrap;" vertex="1" parent="N7N4YLxj38OcdQxVAtvY-11">
          <mxGeometry y="50" width="170" height="140" as="geometry" />
        </mxCell>
        <mxCell id="N7N4YLxj38OcdQxVAtvY-13" value="Review" style="swimlane;childLayout=stackLayout;horizontal=1;startSize=50;horizontalStack=0;rounded=1;fontSize=14;fontStyle=0;strokeWidth=2;resizeParent=0;resizeLast=1;shadow=0;dashed=0;align=center;arcSize=4;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="360" y="570" width="160" height="190" as="geometry" />
        </mxCell>
        <mxCell id="N7N4YLxj38OcdQxVAtvY-14" value="+review_id&lt;div&gt;+property_id&lt;/div&gt;&lt;div&gt;+user_id&lt;/div&gt;&lt;div&gt;+rating(1-5)&lt;/div&gt;&lt;div&gt;+comment&lt;/div&gt;&lt;div&gt;+created_at&lt;/div&gt;" style="align=left;strokeColor=none;fillColor=none;spacingLeft=4;spacingRight=4;fontSize=12;verticalAlign=top;resizable=0;rotatable=0;part=1;html=1;whiteSpace=wrap;" vertex="1" parent="N7N4YLxj38OcdQxVAtvY-13">
          <mxGeometry y="50" width="160" height="140" as="geometry" />
        </mxCell>
        <mxCell id="N7N4YLxj38OcdQxVAtvY-15" value="Message" style="swimlane;childLayout=stackLayout;horizontal=1;startSize=50;horizontalStack=0;rounded=1;fontSize=14;fontStyle=0;strokeWidth=2;resizeParent=0;resizeLast=1;shadow=0;dashed=0;align=center;arcSize=4;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="630" y="570" width="170" height="190" as="geometry" />
        </mxCell>
        <mxCell id="N7N4YLxj38OcdQxVAtvY-16" value="+message_id&lt;div&gt;+sender_id&lt;/div&gt;&lt;div&gt;+recipient_id&lt;/div&gt;&lt;div&gt;+message_body&lt;/div&gt;&lt;div&gt;+sent_at&lt;/div&gt;" style="align=left;strokeColor=none;fillColor=none;spacingLeft=4;spacingRight=4;fontSize=12;verticalAlign=top;resizable=0;rotatable=0;part=1;html=1;whiteSpace=wrap;" vertex="1" parent="N7N4YLxj38OcdQxVAtvY-15">
          <mxGeometry y="50" width="170" height="140" as="geometry" />
        </mxCell>
      </root>
    </mxGraphModel>
  </diagram>
</mxfile>
